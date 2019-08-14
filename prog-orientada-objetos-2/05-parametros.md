# **Programação** Orientada a Objetos 2

## Anotações do professor Lucas Bueno

### Última atualização: 07/08/2019

#### Parâmetros:

- Para obtermos a referência da janela de um controller:

  ```java
  @FXML
  Button botaoDoMeio;
  public void metodoA() {
  	Stage janela = (Stage) botaoDoMeio.getScene().getWindow();
  	janela.close();
  }
  ```

- Para descobrirmos a "fonte" de um evento:
  ```java
  public void tratarClique(ActionEvent e) throws IOException {
		Button botaoClicado = (Button) e.getSource();
		tratarClique(botaoClicado);
		Stage stage = new Stage();
		stage.setScene(new Scene(loadFXML("settings")));
		stage.show();
	}
  ```
- Para passarmos parâmetros para o controller de um FXML:

  

- Para adicionarmos listas nos nossos componentes:

  

- O projeto está disponível em:

  - https://github.com/lucasbueno/projetos-poo2/tree/master/AnchorPaneFXML