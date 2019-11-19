
#### Histórico de revisões
|   Data   |  Versão  |        Descrição       |          Autor(es)          |
|:--------:|:--------:|:----------------------:|:---------------------------:|
|02/09/2019|   0.1    | Iniciando o documento       |  João Gabriel  |
|03/09/2019|   0.2    | Passando Introspecção Iniciativas extras     |  João Gabriel  |
|04/09/2019|   0.3    |  Continuando documento       |  João Gabriel  |
|12/09/2019|   0.4    | Adicionando Épicos       |  João Gabriel e Caue  |
|13/09/2019|   0.5    | Adicionando História de Usuário| João Gabriel e Lucas Gomes|
|18/11/2019|   1.0    | Correção de alguns erros na elicitação de requisitos | [Cauê](https://github.com/caue96) |



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

* **Should**: Segundo nível de prioridade. Requisitos importantes para o projeto.

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
|UC01| - Cadastrar-se no Cafofo| Must | Autenticação |
|UC02| - Cadastrar-se no Cafofo com o Facebook| Could | Autentificação |
|UC03| - Cadastrar-se no Cafofo com o Google| Could | Autentificação |
|UC04| - Visualizar anúncios.| Must | Pesquisa |
|UC05| - Buscar cafofo por localidade| Must | Pesquisa|
|UC06| - Filtrar por avaliações de anúncio| Should | Pesquisa|
|UC07| - Visualizar anúncios de cafofos.| Must | Anúncios |
|UC08| - Visualizar perfil de anunciante| Could | Perfis|
|UC09| - Visualizar avaliações de anunciante| Should | Perfis |
|UC10| - Favoritar anúncio de cafofo| Could | Anúncios |
|UC11| - Avaliar cafofo | Should | Anúncios |
|UC12| - Alterar dados pessoais| Should | Perfis |
|UC13| - Acessar Perfil de Usuário| Must | Perfis |
|UC14| - Filtrar cafofo por valor| Would | Pesquisa |
|UC15| - Efetuar login no Cafofo| Must | Autenticação |
|UC16| - Efetuar login no Cafofo com Facebook| Must | Autenticação |
|UC17| - Efetuar login no Cafofo com Google| Must | Autenticação |
|UC18| - Deslogar do site Cafofo| Must | Autenticação |
|UC19| - Filtrar cafofo por gênero  (Misto/Feminino/Masculino)| Should | Pesquisa |
|UC20| - Filtrar cafofo por contas inclusas | Could | Pesquisa |
|UC21| - Filtrar cafofo por nome| Should | Pesquisa |
|UC22| - Clicar no link para conversa com anunciante/usuário| Should | Comunicação |
|UC23| - Criar anúncio de vaga em cafofo| Must  | Anúncio |
|UC24| - Alterar dados do anúncio do cafofo| Should | anúncio |
|UC25| - Adicionar dados ao anúncio| Must | Anúncio |
|UC26| - Avaliar anunciante| Should | Perfis |
|UC27| - Adicionar usuário ao perfil de membros do cafofo| Could | Anuncio/Perfis |
|UC28| - Adicionar comentário sobre cafofo| Could | Comunicação |
|UC29| - Avaliar Anunciante | Should | Perfis |


## 5. Conclusão

Com base nas tecnicas citadas acima foi criado uma melhor noção e assim levantados os requisitos funcionais do projeto. Tendo em vista que o mesmo será uma aplicação web, com 'CRUD' dos quartos/repúblicas a serem alugados. E um cadastro de usuários sendo divididos em dois tipos: quem aluga e quem loca.<br>
Os requisitos elicitados foram feito no início do projeto em um brainstorm realizado entre os membros do grupo. Com isso esses requisitos inicialmente levantados acabaram ficando obsoleto com relação aos requisitos presentes no [Backlog do Cafofo](https://desenho-2019.github.io/Wiki/Iniciativas%20extras/backlog/). O último ajuste realizado nesse documento foi com o intuito de corrigir alguns erros que foram cometidos na elicitação inicial dos requisitos.
