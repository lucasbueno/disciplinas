# Padrões de projeto

## Anotações do professor Lucas Bueno

#### Última atualização: 19/02/2020

#### Padrões baseados em herança
- “Entidades de software devem ser abertas a extensão, mas fechadas a modificação” - Bertrand Meyer

#### O padrão Null Object
- Em diversas situações em que nosso código depende de um “recurso” que, se não estiver disponível, encheríamos nosso código de “ifs”;

#### O Hook Method
- Até o momento, utilizamos herança para, na classe filha, utilizar os atributos ou métodos da classe mãe. Está é uma abordagem interessante, mas ainda inocente;
- Agora, faremos com que a classe mãe utilize métodos que obrigatoriamente devem ser escritos pela classe filha. Assim podemos ter um algoritmo que será executado com passos que podem ser alterados.
- Se utilizarmos o qualificador *abstract*, a classe filha obrigatoriamente precisará implementar o método. Se utilizarmos o qualificador *protected* e mantivermos o código em branco, a classe filha poderá opcionalmente sobrescrever o método.

#### O Template Method
- Um método que, em sua sequência de etapas, chama outros que devem ser implementados (ou que podem ser implementados) pela classe filham é um template method.

### Referências

- Design Patterns com Java: projeto orientado a objetos guiado por padrões. Eduardo Guerra. Casa do código. 2018.