# Testes de software

## Anotações do professor Lucas Bueno

### Última atualização: 10/05/2020

### Analisadores dinâmicos de código: cobertura

- Na disciplina de testes, dizemos que temos testes estáticos e testes dinâmicos;
    - Os **testes dinâmicos** acontecem durante a execução do programa;
    - já os **testes estáticos** acontecem com a análise do código fonte.
- Um exemplo de teste (ou análise) dinâmica de código é o nosso já conhecido *debugger* 
- Outro exemplo é a **cobertura de código**
    - A cobertura de código pode ser vista como uma métrica que diz quantas linhas do nosso código foram executadas
    - É uma métrica útil para análise do quanto do nosso foi “coberto” por testes unitários
        - Por exemplo: 47% do nosso código é testado através de testes unitários
    - Mas atenção: a qualidade dos testes é tão importante quanto a cobertura: 
        - De nada adianta termos um código 100% coberto por testes de baixa qualidade;
        - De maneira semelhante, de pouco adianta termos testes excelentes mas que cobrem apenas 1% do código.
- A ferramenta EclEmma do Eclipse serve para realizar a cobertura do código
    - Tenho certeza que vocês já a usaram, mas sem querer
    - Também tenho certeza que ficaram muito chateados por não terem entendido o que aconteceu
    - Quando executamos o EclEmma, nos deparamos com uma tela semelhante a esta:
	![https://www.eclemma.org/images/screen.png](../../../screen.png)
    - O significado disso tudo é que as linhas em verde foram cobertas, e as em vermelho não, além das estatísticas de coibertura de cada classe na aba “Coverage”
- Sendo assim, a tarefa desta ferramenta será a seguinte:
    - Estudar o guia do usuário do EclEmma disponível em: https://www.eclemma.org/userdoc/index.html
    - Executar o EclEmma no projeto sobre o JUnit que vocês entregaram na etapa 1 da disciplina
    - Gravar um vídeo mostrando a execução do EclEmma no projeto sobre o JUnit e, no vídeo, explicar os resultados
    - Postar o vídeo no Youtube e me enviar o link no Moodle.
