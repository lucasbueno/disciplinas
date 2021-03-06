# **Programação** Orientada a Objetos 2

## Anotações do professor Lucas Bueno

### Última atualização: 28/10/2020

#### JavaFX com FXML:

- Neste semestre vamos continuar trabalhando com o Java mais atual, que, no caso, é o 14. O professor utilizará o OpenJDK, mas se você preferir, também pode utilizar o JDK da Oracle. No entanto, o uso do **Eclipse** é **mandatório**!

- **Sendo assim, caso precise, baixe a última versão do Java e a última versão do Eclipse**

- Lembre-se de configurar o *Path* nas variáveis de ambiente
- Vamos começar rodando o HelloWorld do JavaFX com FXML utilizando o Maven, para tanto:
	- Crie um projeto Maven seguindo **exatamente** estes passos:
		- File -> New -> Project... -> Maven -> Maven project
		- Selecione o local onde quer salvar o projeto e clique em *Next*
		- Na tela de *Select an Archetype*, selecione *Add Archetype...* e informe: 
			- Group id: org.openjfx
			- Artifact id: javafx-archetype-fxml 
			- Version: 0.0.5
		- O Maven fará o download do arquétipo do projeto, clique em *Next*
		- Em groupid coloque o pacote que preferir (ex.: br.edu.ifsc.canoinhas.poo2), assim como em artifactid (ex.: steam)
		- Clique em *Finish*
- Com isso, o Maven terá criado um projeto padrão em JavaFX, que usa FXML
- Agora, nós podemos rodar a classe App.java e analisar o programa rodando, assim como as classes e arquivos FXML


