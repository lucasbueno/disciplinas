# **Programação** Orientada a Objetos 1

## Anotações do professor Lucas Bueno

### Última atualização: 08/02/2020

- Objetos são acessados por **referências**
    - Um **objeto** da classe **Pessoa** terá uma **referência** para um **objeto** da classe **Endereço**, por exemplo
    - O conceito de **referência** é parecido com o conceito de **ponteiro** (só que mais simples, hehe) 
        - Não podemos realizar operações com referências!
    - Podemos ter **N** referências apontando para o mesmo objeto
    - **new** em Java é o **malloc** do C
    - Lembram o que é passagem de parâmetros por **valor** e passagem de parâmetros por **referência**?
        - Com um exemplo, vamos ver como funciona no Java
    - Um sistema orientado a objetos é um grande conjunto de classes que se comunicam (através de chamadas de métodos e passagem de parâmetros), sendo que cada classe tem um único e bem definido propósito
- Encapsulamento
    - A ignorância é uma benção
    - Um dos conceitos mais importantes da orientação a objetos
    - Nos permite tornar atributos e métodos privados para **controlar e garantir a lógica de funcionamento de uma classe**
    - É extremamente importante quando trabalhamos em equipe
- Entrada de dados:
```java
import java.util.Scanner;
public class HelloWorld {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);
        int n = leitor.nextInt();
        String s = leitor.nextLine();
    }
}
```

