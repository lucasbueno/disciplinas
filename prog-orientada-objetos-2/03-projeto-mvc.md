# **Programação** Orientada a Objetos 2

## Anotações do professor Lucas Bueno

### Última atualização: 06/08/2019

#### Criando um projeto MVC em JavaFX:

- Utilizaremos o padrão de projeto MVC (*Model-View-Controller*) em nossos projetos JavaFX, neste padrão de projeto:
    - O **Model** se refere às nossas entidades
    - O **View** se refere às nossas telas em *FXML*
    - O **Controller** se refere às nossas classes de controle do programa
- Gerenciaremos as bibliotecas necessárias através do Maven, portanto:
    - *File -> New -> Other -> Maven -> Maven project*
    - Na tela de seleção do arquétipo (estrutura do projeto):
        - Se o seguinte não existir, clique em Add Archetype e preencha:
            - “org.openjfx” no **group id**
            - “javafx-archetype-fxml” em **artifact id**
            - “0.0.1” em **version**
    - Termine de criar seu projeto e espere o *build* completar
- Nesta aula:
    - Criaremos uma nova janela Main com um TabPane, dois botões e um label
    - Associaremos esta janela a um controlador, ao clicar nos botões, o label é atualizado com o título dos botões
- O projeto está disponível em:
    - https://github.com/lucasbueno/projetos-poo2/tree/master/1stFXML
