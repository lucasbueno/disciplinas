# Testes de software

## Anotações do professor Lucas Bueno

### Última atualização: 29/03/2020

### Analisadores estáticos de código

- Na disciplina de testes, dizemos que temos testes de caixa branca e testes de caixa preta;
    - Nos testes de **caixa branca** nós temos **acesso** ao **código-fonte** do sistema para criar os testes;]
    - já nos testes de **caixa preta** não.
- Da mesma maneira, também dizemos que temos testes estáticos e testes dinâmicos;
    - Os **testes dinâmicos** acontecem durante a execução do programa;
    - já os **testes estáticos** acontecem com a análise do código fonte.
- Podemos dizer que, das duas ferramentas que já trabalhamos:
    - O JUnit é de **caixa branca** e **dinâmico**;
    - enquanto o Selenium é de **caixa preta** e também **dinâmico.**
- Agora, vamos realizar testes estáticos:
    - A análise estática de um código-fonte, principalmente se feita por  programador diferente do que escreveu o código, tem potencial para  reduzir drasticamente a quantidade de erros e possibilidade de falhas;
    - no entanto, é um processo dispendioso.
    - Para facilitar esta análise, existem ferramentas que fazem a **verificação de erros comuns**  em códigos-fonte;
    - alguns exemplos são:
        - PMD;
        - Infer;
        - RIPS.
    - Nós utilizaremos o PMD;
        - O slogan do PMD é "don't shoot the messenger" (não atire no mensageiro);
        - o slogan vem da ideia de que o PMD é o mensageiro que irá nos mostrar uma quantidade significativa de trechos com **potencial para erro** em nosso código.
    - Portanto, para a tarefa desta etapa da disciplina vocês devem:
        - Instalar o PMD no Eclipse;
        - Analisar as opções disponíveis no PMD;
        - Rodar o PMD em um ou mais projetos em Java;
        - Gravar um vídeo descrevendo pelo menos 5 erros diferentes capturados pelo PMD nos seus projetos (mostrando o relatório do PMD e as linhas do código no vídeo);
        - Enviar o vídeo para o Youtube e enviar o link do vídeo aqui na tarefa;
        - *Cada erro descrito valerá 20% da nota.