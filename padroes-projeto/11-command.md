# Padrões de projeto

## Anotações do professor Lucas Bueno

#### Última atualização: 15/05/2020

#### Command pattern:
- O padrão de comando, como o nome diz, representa operações que podem ser feitas no sistema
- Estas operações vão variar dependendo do domínio da aplicação
- Em um carrinho de *e-commerce,* as operações podem ser de:
    - Adicionar um produto
    - Remover um produto
    - Aumentar a quantidade de um produto
    - Adicionar um cupom de desconto
    - E mais importante: estas operações podem variar de acordo com o tipo de produto vendido, como produtos físicos e produtos digitais
        - Nestes casos, o padrão *command* vai permitir que realizemos a extensão/adaptação do nosso sistema em relação às operações, mas mantendo o resto funcionando normalmente
- Em um editor de texto, as operações podem ser de:
    - Inserir um caractere;
    - Colar uma porção de um texto;
    - Inserir uma imagem.

### Referências

- Design Patterns com Java: projeto orientado a objetos guiado por padrões. Eduardo Guerra. Casa do código. 2018.