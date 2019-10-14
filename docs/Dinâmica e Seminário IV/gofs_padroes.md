# GOFs: Bridge e Decorator

#### Histórico de revisões
|    Data    | Versão |       Descrição       |    Autor(es)     |
| :--------: | :----: | :-------------------: | :--------------: |
| 15/09/2019 |  0.1   | Iniciando o documento e adicionando padrões | André Lucas |

## 1. Bridge

### 1.1 Descrição

Bridge é um sinônimo para o idioma "handle/body". Esse padrão separa uma abstração de sua implementação, permitindo que ambas possam variar independente, sendo estabelecida uma ponte (tradução de “bridge”) entre elas.

O padrão Bridge é utilizado quando:

- Deseja uma ligação em tempo de execução da implementação,
- Tem uma proliferação de classes resultante de uma interface acoplada e inúmeras implementações,
- Deseja compartilhar uma implementação entre vários objetos,
- Precisa mapear hierarquias de classe ortogonais.

### 1.2 Exemplo

## 2. Decorator

### 2.1 Descrição

O padrão Decorator é utilizado quando precisa-se anexar responsabilidades dinamicamente sem precisar de uma grande hierarquia de subclasses.
A descrição original do Padrão Decorator é: "O Padrão Decorator anexa responsabilidades adicionais a um objeto dinamicamente. Os decoradores fornecem uma alternativa flexível de subclasse para estender a funcionalidade".

O Padrão Decorator tem como característica o seguinte:

- Os decoradores têm o mesmo supertipo que os objetos que eles decoram;
- Você pode usar um ou mais decoradores para englobar um objeto;
- Uma vez que o decorador tem o mesmo supertipo que o objeto decorado, podemos passar um objeto decorado no lugar do objeto original (englobado);
- O decorador adiciona seu próprio comportamento antes e/ou depois de delegar o objeto que ele decora o resto do trabalho;
- Os objetos podem ser decorados a qualquer momento, então podemos decorar os objetos de maneira dinâmica no tempo de execução com quantos decoradores desejarmos.

### 2.2 Exemplo 


