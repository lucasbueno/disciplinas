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
  ```java
  Stage stage = new Stage();
  FXMLLoader fxmlLoader = new FXMLLoader(App.class.getResource("settings.fxml"));
  Parent root = (Parent) fxmlLoader.load();
  stage.setScene(new Scene(root));
  SettingsController controller = fxmlLoader.getController();
  controller.setParametro(2);
  stage.show();
  ```

- Para adicionarmos listas nos nossos componentes:
  ```java
  private ObservableList<String> nossaLista;
  
  public void nossoMetodo() {
      getNossaLista().add(nossaTxt.getText());
  }
  
  private ObservableList<String> getNossaLista() {
      if (this.nossaLista == null) {
          this.nossaLista = FXCollections.observableArrayList();
          nossaListView.setItems(nossaLista);
      }
      return this.nossaLista;
  }
  ```
  
- O projeto está disponível em:

  - https://github.com/lucasbueno/projetos-poo2/tree/master/AnchorPaneFXML
  
- Para mais informações sobre a ListView:

    - https://docs.oracle.com/javafx/2/ui_controls/list-view.htm