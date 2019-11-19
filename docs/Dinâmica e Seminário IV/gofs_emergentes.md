# GOFs Emergentes

#### Histórico de revisões
|    Data    | Versão |                  Descrição                  |           Autor(es)            |
| :--------: | :----: | :-----------------------------------------: | :----------------------------: |
| 17/10/2019 |  0.1   | Iniciando o documento e adicionando padrões |André Lucas|
| 18/10/2019 |  0.1   | Adicionando padrão HOC Router |André Lucas|

## 1. Padrões do Django

### 1.1 Documentação

Modelos devem encapsular cada aspecto de um objeto, seguindo o padrão de projeto Active Record de Martin Fowler.

![Active-Record](img/activeRecord.png)

Esse é o porque de ambos os dados representandos por um modelo e a informação sobre eles (seus nomes legíveis, opções como ordenação padrão, etc) são definidos na classe de modelo; toda a informação necessária para entender um dado modelo deveria ser amazenada no modelo.

### 1.2 Padrões comportamentais

|GOF|Componente|Descrição|
| :----: | :----: | :----: |
|Command|HTTP Request|Encapsula uma solicitação em um objeto|
|Observer|Signals|Quando um objeto muda de estado, todos os demais são associados a ele são notificados e atualizados automaticamente|
|Template|Baseado em classes|Etapas de um algoritmo podem ser redefinidas por subclasses sem alterar a estrutura do algoritmo
|

###  1.3 Padrão estrutural

Serializer() é um método nativo do Django Rest que permitem que dados complexos, como querysets e instâncias de modelo, sejam convertidos em tipos de dados Python nativos que podem ser facilmente renderizados em JSON, XML ou outros tipos de conteúdo.

**Adapter :** converte uma interface de uma classe para outra interface que o código cliente espera encontrar. A entidade adaptadora permite que classes com interfaces incompatíveis trabalhem juntas.

## 2. HOC para Router

Digamos que temos algumas páginas em que apenas queremos que usuários autenticados a visualizem, podemos usar o HOC aqui para lidar com isso.

```
const PrivateRoute = ({ component: Component, ...rest }) => (
    <Route
      {...rest}
      render={props =>
        isAuthenticated() ? (
          <Component {...props} />
        ) : (
          <Redirect to={{ pathname: "/", state: { from: props.location } }} />
        )
      }
    />
  );
```

Então, uma função que recebe um Component retorna AuthenticatedComponent, além de verificar se o usuário já está autenticado; caso contrário, ele será redirecionado para /home.

Agora, podemos usar o HOC e atualizar onde definimos as rotas:

```
<Switch>
    <Route exact path="/" component={Main} />
    <Route path="/login" component={Login} />
    <PrivateRoute path="/cafofos/:id" component={Adsinfo} />
    <PrivateRoute path="/cafofos" component={Adslist} />
    <PrivateRoute path="/register-cafofo" component={AdsRegister} />
    <Route path="/cadastro" component={UserRegister} />
    <Route path="/esqueci-a-senha" component={ForgotPassword} />
    <Route path="*" component={() => <h1>Page not found!</h1>} />
</Switch>
```

## Referências

- [Django](https://docs.djangoproject.com/pt-br/2.2/misc/design-philosophies/)
