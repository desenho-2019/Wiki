# Plano de Gestão e Configuração de Software

## Histórico de Revisão

|   Data   |  Versão  |        Descrição       |          Autor(es)          |
|:--------:|:--------:|:----------------------:|:---------------------------:|
|31/08/2019|   0.1    | Criação do Documento de GCS           |  [Rafael](https://github.com/rafaelbrg) |
|02/09/2019|   0.2    | Adicionada Introdução e Itens de Configuração  |  [Rafael](https://github.com/rafaelbrg) |
|02/09/2019|   0.3    | Adicionada Politica de commits |  [Rafael](https://github.com/rafaelbrg) |
|03/09/2019|   0.4    | Adicionada Politica de branchs |  [Rafael](https://github.com/rafaelbrg) |

## 1. Introdução

<p align = "justify">Este documento tem como finalidade estabelecer os procedimentos de gerência e configuração de software a serem seguidos no projeto.</p>

## 2. Itens de Configuração

<p align = "justify">A preocupação da equipe, referente à configuração, é voltada para a documentação textual e o código. Estes são dispostos conforme o seguinte:</p>

* Código: Todo e qualquer artefato que seja composto de uma ou mais linguages de programação.

* Documento: Todo e qualquer artefato textual que contenha informações da matodologia, planejamento, produto, integração da equipe, reuniões e demais informações pertinentes ao processo de desenvolvimento do produto.

## 3. Políticas

### 3.1 Política de Commits

* <p align = "justify">Os commits devem ser criados logo em seguida à finalização de um conjunto conexo de alterações, descrevendo-o de forma sucinta e atômica. O texto deve descrever o que foi produzido, de forma resumida e em <b>inglês</b>, com o tempo verbal no particípio. Como no seguinte formato:

* Texto começando com letra maiúscula e com o verbo no particípio.

* Exemplo:

   ```Updated product logo```

</p>

* Commits devem ser redigidos no idioma inglês
* Devem ser simples e concisos, possuindo títulos curtos
* Commits devem descrever o que está sendo alterado, se houver mais de uma alteração (pertinente ao commit) ela deve ser adicionada na descrição do commit
* Devem iniciar com letras maiúsculas.
* Devem iniciar com um verbo no particípio informando seu objetivo. Ex: "Deleted old files"

### 3.2 Política de Branches

<br>

[![img](img/imgg)](img/img)

<br>

* <p align = "justify"> A <i>Master</i> será a branch principal do projeto em um dado repositório.</p>

* <p align = "justify">A <i>Master</i> será a branch estável do projeto e só sera atualizada, a partir da branch <i>development<i>, quando um <i>pull request<i> for aceito. É proíbido que membros subam commits diretamente na <i>Master</i>.</p>

 * A única exceção para essa régra sera no repositório da Wiki.

* <p align = "justify">As branches auxiliares são para a resolução das funcionalidades ou correções de erro. Cada <i>Tarefa</i> ou <i>bugfix</i> terá sua própria branch, criada a partir da branch <i>development</i>, e terá como nomenclatura o seguinte padrão: </p>

   ``` TF[ID da Tarefa no RoadMap]-[Nome da Tarefa] ``` ou <br>
   ``` FIX[ID da issue a ser resolvida]-[Nome da issue] ``` ou <br>
   ``` FIX[Nome da correcao ou configuracao] ``` ou <br>
   ``` TE-[Nome da Tarefa Extra] ```<br>

* Para cada Feature uma nova branch deve ser criada com base no último commit da develop.
