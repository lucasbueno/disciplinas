# Padrões de projeto

## Anotações do professor Lucas Bueno

#### Última atualização: 09/02/2020

![Resultado de imagem para estratégia em grego](02-strategy.assets/Estratégia.jpg)

**"Por mais brilhante que seja a estratégia, você deve sempre olhar para os resultados." Winston Churchill.**

- Devemos utilizar o padrão Strategy sempre que o problema envolver a escolha de um entre diversos algoritmos, sendo que cada algoritmo é o adequado apenas para um conjunto de situações
- Por exemplo: as diferentes instituições de ensino possuem regras diferentes para o cálculo da nota final dos alunos. Mais ainda, em uma mesma instituição de ensino, os professores possuem métodos diferentes para calcular a nota final dos alunos (que obedecem a da instituição, a princípio). Como desenvolver um sistema acadêmico genérico, que seja adaptável para todas as instituições e professores?
- Outro exemplo: o preço dos estacionamentos de veículos, em geral, varia de acordo com o tipo do veículo, o tipo de contrato e o tempo de permanência do veículo. Como desenvolver um sistema para controle de estacionamentos genérico, que seja adaptável para todos que o queiram comprar?
- E o último exemplo: o cálculo do imposto de renda, além de sofrer constantes alterações, depende da faixa salarial em que a renda da pessoa se enquadra, do tipo de cálculo escolhido (simplificado ou não), dos diversos ganhos, etc. Como desenvolver o sistema para cálculo do imposto de renda de forma que ele seja facilmente adaptável no futuro?

![https://robsoncastilho.files.wordpress.com/2011/04/strategy.gif?w=616](02-strategy.assets/strategy.gif)

### Referências

- Design Patterns com Java: projeto orientado a objetos guiado por padrões. Eduardo Guerra. Casa do código. 2018.