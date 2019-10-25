# GOFS Emergentes

#### Histórico de revisões
|    Data    | Versão |       Descrição       |    Autor(es)     |
| :--------: | :----: | :-------------------: | :--------------: |
| 18/10/2019 |  0.1   | Iniciando o documento | André Lucas |

## 1. Facade

Prover uma interface simplificada para a utilização de várias interfaces de um subsistema.


### 1.1 Estrutura Genérica

![Estrutura-Facade](img/Facade.png)

### 1.2 Utilização no projeto Cafofo

Seguindo boas práticas de implementação do Django, é possível identificar tal padrão de projeto dentro do arquivo urls.py. Onde na aplicação existem vários apps, e cada um possui seu arquivo url, sendo o ulrs.py do projeto uma fachada para chamar as outras urls.py de cada app.

##### Implementação
```
# cafofo_api urls.py 

"""cafofo_api URL Configuration

The `urlpatterns` list routes URLs to views. For more information please see:
    https://docs.djangoproject.com/en/2.2/topics/http/urls/
Examples:
Function views
    1. Add an import:  from my_app import views
    2. Add a URL to urlpatterns:  path('', views.home, name='home')
Class-based views
    1. Add an import:  from other_app.views import Home
    2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
Including another URLconf
    1. Import the include() function: from django.urls import include, path
    2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
"""
from django.contrib import admin
from django.urls import path,include
from rest_framework import routers
from django.conf.urls.static import static
from django.conf import settings

router = routers.DefaultRouter()


urlpatterns = [
    path('admin/', admin.site.urls),
    path('', include(router.urls)),
    path('api-auth/', include('rest_framework.urls', namespace='rest_framework')),
    path('user/',include('users.urls')),
   ] + static(settings.MEDIA_URL, document_root= settings.MEDIA_ROOT)


   # users urls.py

   from django.conf import settings
from django.conf.urls.static import static
from django.urls import path,include

from users.views import  ExampleView,  ListUser, CreateUser,UserUpdateDeleteSet
from rest_framework_simplejwt.views import TokenObtainPairView,TokenRefreshView





urlpatterns = [
    path('api/token/', TokenObtainPairView.as_view(), name='token_obtain_pair'),
    path('api/refresh/', TokenRefreshView.as_view(), name='token_refresh'),
    path('exemple/', ExampleView.as_view()),
    path('list/',ListUser.as_view()),
    path('create/',CreateUser.as_view()),
    path('settings/<int:pk>/',UserUpdateDeleteSet.as_view()),
   ] + static(settings.MEDIA_URL, document_root= settings.MEDIA_ROOT)
```


## 2. Template Method
Defina o esqueleto de um algoritmo em uma operação, adiando algumas etapas para as subclasses do cliente. Template Method permite que as subclasses redefinam certas etapas de um algoritmo sem alterar a estrutura do algoritmo.

### 2.1 Estrutura Genérica
![Estrutura-TemplateMethod](img/Template_Method.png)

### Utilização no Projeto Cafofo
Essa estrutura comumente é utilizada nos forms dos apps em django, onde se define os campos que estarão presentes em determinados formulários. Contudo, por se tratar de uma api, os campos delimitados a estarem presentes em determinados "formulário" foi definidos no serializer.py de cada app.

```
from rest_framework import serializers
from users.models import CustomUser

class UserSerializer(serializers.ModelSerializer):
    class Meta:
        model = CustomUser
        fields = [ 'id','email','password','name','phone','date_of_birth','gender','nationality','facebook','google','photo']


class UserCreateUpdateSerializer(serializers.ModelSerializer):
    password = serializers.CharField(
        style ={'input_type':'password'}
    )
    class Meta:
        model = CustomUser
        fields = ['email','password','name','phone','date_of_birth','gender','nationality','facebook','google','photo',]
```

## Referências

https://refactoring.guru/design-patterns/facade