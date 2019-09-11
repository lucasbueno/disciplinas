# **Programação** Orientada a Objetos 2

## Anotações do professor Lucas Bueno

### Última atualização: 11/09/2019

#### Object-relational Mapping (ORM):

- Técnica para mapear um modelo orientado a objetos em um modelo relacional
  - O programador interage com a API, e as consultas SQL são abstraídas
  - Mas quais as diferenças entre estes dois modelos?
    - Um dos principais focos do modelo relacional é possibilitar a recuperação rápida das informações
        - Por mais que isso possa não ser muito aderente a como as informações são entendidas no mundo real
        - Um avalista de crédito, no mundo real, pode ser tanto uma pessoa física quanto uma pessoa jurídica, por exemplo.
    - Já no modelo orientado a objetos, o foco é em manter a estrutura o mais parecida possível com a representação do mundo real
        - Um cliente e um funcionário não precisam ter um ID para dizermos que um determinário funcionário fez uma venda para um determinado cliente, por exemplo
    - Por isso o ideal é armazenar os dados em um banco relacional, mas escrever o código (que provavelmente demandará bastante manutenção) no modelo orientado a objetos
        - O que poderia ser uma grande dor de cabeça para os programadores, que precisariam ora trabalhar com um modelo, ora com outro
        - Mas felizmente existe ORM!
- Existem vários *frameworks* para utilizarmos ORM, e eles são específicos para cada linguagem, um dos mais antigos e famosos é o **Hibernate** - que é o que iremos utilizar
- Mas antes disso, vamos conhecer um histórico da manipulação de bancos de dados com a linguagem de programação Java:
  - ODBC: uma API que define como um programa pode acessar um banco de dados
  - JDBC: uma API que define como um progama Java pode acessar um banco de dados
      - Começou a ser desenvolvida em 1997 e hoje está na versão 4.3
      - Para abrir uma conexão você informa o endereço, o usuário, a senha e o *driver* JDBC
  - JPA:  *Java Persistence API*, nasceu como resposta ao Hibernate, mas hoje é possível utilizar o Hibernate pela especificação JPA
      - É uma especificação, e existem várias implementações, a implementação de referência é a EclipseLink, mas utilizaremos o **Hibernate**
- E antes de ir ao código, precisamos definir qual banco de dados vamos utilizar
    - Uma das mágicas em utilizar tecnologias como o Hibernate e JPA, é que elas permitem realizar a troca dos bancos de dados de maneira rápida, fácil e transparente
    - Outra grande mágica é que não precisaremos nos preocupar com o gerenciamento dos recursos do banco de dados, como abertura e fechamento de conexões
    - Nos exemplos da disciplina utilizarei o **SQLite**, uma *engine* para criação de bancos de dados relacionais, onde:
      - tudo fica salvo em um único arquivo autocontido, o que é:
        - rápido
        - portátil (funciona em qualquer plataforma)
        - leve (a *engine* pesa cerca de 600KiB)
        - talvez menos confiável
        - talvez menos seguro
        - talvez pior para múltiplos acessos
      - normalmente cada aplicativo que roda em seu *smartphone* salva suas informações em um bancos de dados SQLite, mas também normalmente fazendo um *backup* na nuvem
      - existem mais de 1 trilhão de bancos de dados SQLite em uso no mundo
      - para navegarmos em bancos de dados feitos com o SQLite, podemos utilizar o [DB Browser for SQLite](https://sqlitebrowser.org/)