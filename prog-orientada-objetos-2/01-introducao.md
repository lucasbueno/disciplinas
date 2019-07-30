# **Programação** Orientada a Objetos 2

## Anotações do professor Lucas Bueno

### Última atualização: 22/07/2019

#### JavaFX com FXML:

- Neste semestre, já mais avançados, vamos trabalhar com o Java 11 (ou se preferir, o Java 12). O professor utilizará o OpenJDK, mas se você preferir, também pode utilizar o JDK da Oracle. No entanto, o uso do **Eclipse** é **mandatório**!

- Vamos começar rodando o HelloWorld do JavaFX com FXML utilizando o Maven, para tanto:

  - Crie um Maven Project assim:

    - File -> New -> Project... -> Maven -> Maven project
    - Na tela de "Select an Archetype", selecione "Add Archetype..." e informe: 
      - Group id: org.openjfx
      - Artifact id: javafx-archetype-fxml 
      - Version: 0.0.1
    - Na tela de "Specify Archetype parameters", em Group Id coloque o package que preferir (ex.: br.edu.ifsc.canoinhas.poo2), e em "Artifact Id" coloque como nome do projeto também o que preferir

  - Adicione o seguinte código no pom.xml, dentro da tag <plugins>:

    ```xml
    <plugin>
        <groupId>org.openjfx</groupId>
        <artifactId>javafx-maven-plugin</artifactId>
        <version>0.0.2</version>
        <configuration>
            <mainClass>HelloFX</mainClass>
        </configuration>
    </plugin>
    ```

    

