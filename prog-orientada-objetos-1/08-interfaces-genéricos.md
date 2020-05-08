# **Programação** Orientada a Objetos 1

## Anotações do professor Lucas Bueno

### Última atualização: 08/05/2020

#### Interfaces:
- Uma interface funciona como um contrato entre as classes. Nela, adicionamos apenas a assinatura dos métodos que as classes que forem seguir este contrato precisam implementar
- Desta forma, podemos utilizar o polimorfismo dizendo que nossa referência é do tipo InterfaceDAO, sendo que o objeto em si poderá ser de qualquer classe que implemente o contrato InterfaceDAO

#### Tipos genéricos:
- Ao declarar um <Tipo> genérico ao lado do nome da classe, estamos dizendo que esta classe poderá ser utilizada para qualquer tipo de objeto
- É assim que as classes List<T> e ArrayList<T> funcionam também com classes que nós criamos.