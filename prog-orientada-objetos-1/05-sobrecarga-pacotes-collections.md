# **Programação** Orientada a Objetos 1

## Anotações do professor Lucas Bueno

### Última atualização: 09/03/2020

#### Sobrecarga de métodos:

- Métodos podem ser sobrecarregados, desde que possuam parâmetros diferentes
    - A assinatura de um método é composta pelos modificadores + retorno + nome + parâmetros
    - Então para sobrecarregar um método, tudo deve ser igual, com exceção dos parâmetros
    - Podemos sobrecarregar inclusive os métodos construtores (e é muito útil)
        - Com este artifício fica fácil definir restrições sobre como podemos e sobre como não podemos criar um objeto
```java
import java.util.Scanner;
public class Teste {
    private String nome;
    private int idade;
    
    public Teste(String nome){
        this.nome = nome;
    }
    
    public Teste(String nome, int idade){
        this.nome = nome;
        this.idade = idade;
    }
}
```
#### Pacotes:

 - Pacotes fazem parte da assinatura de uma classe
     	
     - Eles possibilitam a existência de duas classes com o mesmo nome, por exemplo
        - E é claro, auxiliam na organização do código
        - O padrão é utilizar o website da organização "ao contrário", como: br.com.lucasbueno 
     
#### Collections:
 - É um pacote de classes com estruturas de dados prontas
 - São muito úteis e existem estruturas específicas para cada situação
 - Por enquanto, vamos começar com as seguintes:
     - https://docs.oracle.com/en/java/javase/13/docs/api/java.base/java/util/ArrayList.html
     - https://docs.oracle.com/en/java/javase/13/docs/api/java.base/java/util/HashMap.html