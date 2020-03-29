# Testes de software

## Anotações do professor Lucas Bueno

### Última atualização: 29/03/2020

### Ferramentas de captura e reprodução

- As ferramentas de captura e reprodução servem para as **situações** em **que** os **testes unitários não são suficientes**, em geral para **simularmos** a **interação** dos usuários com a **interface gráfica**;

- Pela natureza deste tipo de ferramenta, elas são altamente dependentes das tecnologias que queremos testar;

- Alguns exemplos de ferramentas:

    - Selenium (para testar a interação com sites);
    - MoneyRunner (para testar a interação com apps no Android);
        - O que não exclui a possibilidade de utilizarmos JUnit para criar testes unitários para nossos apps Android;
    - Sikuli (web/mobile)
    - Espresso (também para testar a interação com apps no Android).

- Estas ferramentas, de uma maneira geral, são bem simples. Nelas, criamos 

    scripts 

    que representam uma sequência de interações com nosso software, algo como:

    - Clique no botão com id "btnNewUser";
    - Digite "lucasbueno" na caixa de texto com id "txtUsername";
    - Clique no botão com id "btnSave".

- Assim, toda vez que quisermos analisar uma interação, basta rodarmos o script. Podemos até mesmo rodar o script em um tempo bastante rápido, algo como 2x ou 3x o tempo que levaríamos se realizássemos a interação  manualmente;

    - Aliás, nesta altura vocês já devem estar cansados de rodar os  programas de vocês e ficar clicando e digitando alguns testes pra  descobrir que tem erro e depois fazer de novo, e de novo... hehe

- E finalmente, a tarefa deste conteúdo é:

    - Aprender a utilizar o Selenium IDE
        - Que é uma extensão que pode ser utilizada tanto no Firefox quanto no Google Chrome
        - E que está disponível aqui: https://www.selenium.dev/downloads/
    - Escolher um site com o qual seja possível realizar interações complexas (de login, configuração de perfil, etc.), como:
        - SIGAA
        - Steam
        - Facebook
    - Fazer um vídeo gravando a tela do seu computador e no qual você  explica o funcionamento da ferramenta através da criação e da execução  de um script no site escolhido;
    - Publicar o vídeo no Youtube e enviar o link aqui no Moodle.