
#### Histórico de revisões
|   Data   |  Versão  |        Descrição       |          Autor(es)          |
|:--------:|:--------:|:----------------------:|:---------------------------:|
|02/09/2019|   0.1    | Iniciando o documento       |  João Gabriel  |
|03/09/2019|   0.2    | Passando Introspecção Iniciativas extras     |  João Gabriel  |
|04/09/2019|   0.3    |  Continuando documento       |  João Gabriel  |
|12/09/2019|   0.4    | Adicionando Épicos       |  João Gabriel e Caue  |
|13/09/2019|   0.5    | Adicionando História de Usuário| João Gabriel e Lucas Gomes| 



# Elicitação de requisitos funcionais

## 1. Objetivo

O objetivo visado neste documento é levantar os requisitos funcionais que serão desenvolvidos ao longo do segundo semestre letivo de 2019. Identificando assim as necessidades dos stakeholdes para que assim possa ser priorizado o desenvolvimento e se adequar ao tempo disponível.

## 2. Técnicas utilizadas
Ao longo da primeira dinâmica executada na matéria foram feitas algumas tecnicas de elicitação a fim de criar uma noção sobre o projeto a ser desenvolvido. Foram elas:

* 5w2H
* Mapa mental
* Rich Picture
* Prototipação


Contudo, uma outra tecnica será utilizada nesta fase do projeto (Dinâmica e Seminario II) a Introspecção.

## 3. Modelo de Priorização

A partir dos requisitos levantados pelas diversas técnicas utilizadas pelo time, serão priorizados de acordo com necessidade dos mesmos para o projeto seguindo o modelo de priorização MoSCoW. Tal modelo classifica os requisitos em uma escala pré definida, sendo ela:

* **Must**: Primeiro nível de prioridade. Requisitos essencias para o projeto

* **Shuld**: Segundo nível de prioridade. Requisitos importantes para o projeto.

* **Could**:Terceiro nível de prioridade. Requisitos interesantes para o projeto.

* **Would**: Quarto nível de prioridade. Requisitos desejáveis ao projeto

## 4. Épicos

### EP01
#### Perfis
Permitir que usuários criem e alterem dados de suas respectivas contas.

### EP02
#### Anúncios
Permitir que usuário-anunciante crie e altere dados referentes ao local.

### EP03
#### Pesquisa
Criar funcinonalidade que permita que qualquer usuário cadastrado ou não, possa efetuar pesquisa de locais.

### EP04
#### Autenticação
Criar funcionalidades de autenticar usuários.

### EP05
#### Comunicação
Criar meio de comunicação locador e locatário dentro da plataforma .


## 5. História de usuário


|US| Descrição|Priorização| Épico
|:----:|:-------:|:-------:|:-----:|
|UC01| - Cadastrar-se no Cafofo| Must  | Autenticação |
|UC02| -Visualizar cafofos.| Must | Pesquisa |
|UC03| - Visualizar o Menu de Configurações| Should |Perfis |
|UC04| - Buscar cafofo por localidade| Must | pesquisa|
|UC05| - Configurar outras notificações| Would |-- |
|UC06| - Visualizar avaliações de cafofos| Should | Anúncios|
|UC07| - Visualizar Anúncios de cafofos.| Must | Anúncios |
|UC08| - Visualizar perfil de anunciante| Could | Perfis|
|UC09| - Visualizar avaliações de anunciante| Should | Perfis |
|UC10| - Compartilhar anúncio de cafofo| Must | Anúncios |
|UC11| - Favoritar anúncio de cafofo| Could | Anúncios |
|UC12| - Avaliar cafofo | Should | Anúncios |
|UC13| - Alterar dados pessoais| Should | Perfis | 
|UC14| - Acessar Perfil de Usuário| Must | Perfis |
|UC15| - Filtrar cafofo por valor| Would | Pesquisa |
|UC16| - Efetuar login no Cafofo| Must | Autenticação |
|UC17| - Deslogar do site Cafofo| Must | Autenticação |
|UC18| - Solicitar contato| Would | Comunicação | 
|UC19| - Filtrar cafofo por genero  (Misto/Feminino/Masculino)| Should |Pesquisa |
|UC20| - Filtrar cafofo por inclusões (incluso água, luz, internet...)| Could | Pesquisa |
|UC21| - Filtrar cafofo por nome| Should | Pesquisa |
|UC22| - Filtrar cafofo por recomendações| Could | Pesquisa |
|UC23| - Limpar histórico de Busca| Would |-- |
|UC24| - Clicar no link para conversa com anunciante/usuário| Should | Comunicação |
|UC25| - Criar perfil do cafofo| Must | Perfis |
|UC26| - Criar anúncio de vaga em cafofo| Must  | Anúncio |
|UC27| - Alterar dados do cafofo| Must | Perfis |
|UC28| - Alterar dados do anúncio do cafofo| Should | anúncio |
|UC29| - Adicionar fotos ao anúncio| Must | anúncio |
|UC30| - Adicionar localidade ao anúncio| Must |  Anúncio |
|UC31|-  Adicionar descrição ao anúncio| Must | Anúncio |
|UC32| - Adicionar valor do anúncio| Must | Anúncio |
|UC33| - Avaliar perfil do usuário| Should | Perfis |
|UC34| - Adicionar usuário ao perfil de membros do cafofo| Could | Anuncio/Perfis |
|UC35| - Adicionar comentário sobre cafofo| Could | Comunicação |
|UC36| - Avaliar Anunciante | Should | Perfis |




## 5. Conclusão

Com base nas tecnicas citadas acima foi criado uma melhor noção e assim levantados os requisitos funcionais do projeto. Tendo em vista que o mesmo será uma aplicação web, com 'CRUD' dos quartos/repúblicas a serem alugados. E um cadastro de usuários sendo divididos em dois tipos: quem aluga e quem loca.
