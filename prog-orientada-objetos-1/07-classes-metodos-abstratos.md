# **Programação** Orientada a Objetos 1

## Anotações do professor Lucas Bueno

### Última atualização: 09/03/2020

#### Classes abstratas:

- Classes abstratas não podem ser instanciadas
- Elas vão servir como um modelo, para que outras classes possam estender suas funcionalidades, assim como compartilhar atributos e comportamentos

#### Métodos abstratos:

- São métodos apenas com a assinatura, i.e., sem a implementação do método;
- Só podem ser criados em classes abstratas, já que se pudéssemos instanciar uma classe com um método abstrato, o que aconteceria se chamássemos o método não implementado?
- Elas vão servir como uma restrição para as classes que estenderem a classe abstrata que possui o método abstrato. As classes filhas serão obrigadas a implementar o método abstrato