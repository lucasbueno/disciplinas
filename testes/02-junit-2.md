# Testes de software

## Anotações do professor Lucas Bueno

### Última atualização: 17/02/2020

- Assertions: métododos úteis para verificar “afirmações”
    - https://junit.org/junit5/docs/current/api/org.junit.jupiter.api/org/junit/jupiter/api/Assertions.html
    - assertEquals
    - assertNotEquals
    - assertNull
    - assertThrows
    - Agrupamento de Assertions:
    
        ```java
        @Test
        void groupAssertions() {
            int[] numbers = {0, 1, 2, 3, 4};
            assertAll("numbers",
                () -> assertEquals(numbers[0], 1),
                () -> assertEquals(numbers[3], 3),
                () -> assertEquals(numbers[4], 1)
                );
        }
        ```
    
- Anotações úteis:
    - @Test: o método anotado é um teste unitário
    - @BeforeEach: o método anotado será executado antes de cada teste unitário
    - @AfterEach: o método anotado será executado depois de cada teste unitário
    - @BeforeAll: o método anotado será executado antes de todos os testes
    - @AfterAll: o método anotado será executado depois de todos os testes
    - @Disable: o método ou a classe anotada não será executada na execução dos testes 
    - @Timeout: o teste falhará se a execução ultrapassar o tempo informado
    
- Assumptions: métodos úteis para rodar testes apenas se alguma condição for verdadeira

    - https://junit.org/junit5/docs/current/api/org.junit.jupiter.api/org/junit/jupiter/api/Assumptions.html
    - assumeFalse
    - assumeTrue
