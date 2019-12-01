# Matemática aplicada 2

## Anotações do professor Lucas Bueno

### Última atualização: 18/10/2019

#### Probabilidade:

##### Introdução:

 - Nesta etapa da disciplina não estamos mais preocupados em descrever os dados, mas sim em aprender com os dados;
 - Em toda a nossa vida, aprendemos que é ruim fazer **suposições**. Mas se pararmos para pensar, toda a nossa vida depende das supsições;
 - O problema da indução e a falseabilidade;
 - Na teoria da probabilidade, conhecemos o modelo, mas não os dados. Na teoria da estatística, conhecemos os dados, mas não o modelo;

#### Algumas definições:
 - Espaço amostral: o conjunto de todos os possíveis resultados;
 - Evento elementar: um único resultado do espaço amostral;
 - Lei da probabilidade: a soma das probabilidades dos eventos elementares deve somar 1. Assim potemos ter uma distribuição de probabilidade;
 - Eventos não elementares: um ou mais eventos elementares juntos;

#### Regras básicas:
 - Regra do E: um evento independente não afeta a probabilidade de outro evento independente. Portanto, a probabilidade dos dois ocorrerem é a probabilidade do primeiro ocorrer multiplicada pela probabilidade do segundo ocorrer;
 - Regra do OU: a probabilidade de 1 ou outro evento ocorrer, é o somatório da probabilidade de cada evento ocorrer.

##### Exercícios:
 - No lançamento de dois dados perfeitos, qual a probabilidade de que a soma dos resultados obtidos seja igual a 6?
 - Em uma urna existem bolas enumeradas de 1 a 15. Qualquer uma delas possui a mesma chance de ser retirada. Determine a probabilidade de se retirar uma bola com número nas seguintes condições: 
     - par; 
     - primo; 
     - par ou primo; 
     - par e primo.

#### Distribuição binomial:
 - Uma distribuição estatística é uma função que define uma curva de probabilidades;
 - A binomial pode ser usada para calcular a probabilida de que ocorram exatamente um número X de sucessos em N lançamentos aleatórios e independentes, desde que o experimento tenha apenas dois resultados possíveis (sucesso ou fracasso) e que a probabilidade de sucesso se mantenha constante em todos os experimentos;
 - No R, podemos utilizar as funções "dbinom()", “pbinom()”, “rbinom()”.

#### Distribuição normal:
 - Ao contrário da binomial, pode ser utilizada para dados contínuos (como a temperatura);
 - Como já vimos, ela é definida pela média e pelo desvio padrão e:
     - Cerca de 68% dos dados estão entre 1 desvio padrão da média, 95% entre 2 desvios padrões, e 99.7% entre 3 desvios padrões;
- Mas o que acontece se alterarmos a média? E se alterarmos o desvio padrão?
- Muitos experimentos tem o formato de uma distribuição normal e, para estes casos, fica fácil calcular a probabilidade de que uma condição ocorra. Mas mesmo para os experimentos que não possuem o formato da distribuição normal, o teorema central do limite diz que:
     - A distribuição da média dos experimentos converge para uma distribuição normal na medida em que o tamanho das amostras aumenta. Podemos visualizar isso com o exemplo ilustrado aqui: http://www.portalaction.com.br/probabilidades/convergencia-de-variaveis-aleatorias
- No R, podemos utilizar as funções "dnorm()", “pnorm()”, “rnorm()”;
- Site para plotar distribuições normais: https://www.desmos.com/calculator/0x3rpqtgrx


#### Referências bibliográficas:

1. Bruno Fontana da Silva, Jean Diniz e Matias Américo Bortoluzzi. Minicurso de Estatística Básica: Introdução ao Software R. http://www.uft.edu.br/engambiental/prof/catalunha/arquivos/r/r_bruno.pdf
2. Danielle Navarro. Learning statistics with R. http://compcogscisydney.org/learning-statistics-with-r/
3. Marcos Noé Pedro da Silva. Exercícios sobre Propriedades da Probabilidade. https://exercicios.brasilescola.uol.com.br/exercicios-matematica/exercicios-sobre-propriedades-probabilidade.htm#resp-2