# Testes de software

## Anotações do professor Lucas Bueno

### Última atualização: 10/01/2020

- Tipos de testes:
    - Testes de unidade
    - Testes de integração
    - Testes de sistema
    - Testes de aceitação
- Vamos utilizar o **JUnit** no **Eclipse** para automatizar os testes de unidade, de integração e de sistema
- Crie um projeto maven e durante a criação opte por um arquétipo simples
- Crie a classe *Person* dentro de um pacote no estilo "br.com.lucasbueno.entities" que estará dentro de src/main/java
-  Crie um JUnit Test Case (selecione "New JUnit Jupiter test") chamado *PersonTest* dentro de um pacote no estilo "br.com.lucasbueno.entities" (use o mesmo pacote da classe Java), mas que estará dentro de src/**test**/java. Em "Class under test", busque pela classe Java que você criou no passo anterior
    - Você precisará configurar o "project compliance" para pelo menos a versão 8 do java
    - Você precisará adicionar o JUnit 5 no build path (quando clicar em Finish esta opção aparecerá)
- Código da classe Person:
```java
package br.com.lucasbueno.entities;

public class Person {
	
	public String hello() {
		return "hey";
	}

}
```
- Código da classe PersonTest:
```java
package br.com.lucasbueno.entities;

import static org.junit.jupiter.api.Assertions.*;

import org.junit.jupiter.api.Test;

class PersonTest {

	@Test
	void test() {
		Person person = new Person();
		assertEquals("hello", person.hello());
	}

}
```
1. Rode o teste, veja falhar
2. Refatore o código
3. Rode o teste, veja passar