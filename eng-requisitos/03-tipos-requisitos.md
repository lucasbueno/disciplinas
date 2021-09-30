# Engenharia de Requisitos

## Anotações do professor Lucas Bueno

### Última atualização: 30/09/2021

#### Tipos de requisitos
* Para entendermos os diferentes tipos de requisitos, é importante definirmos alguns conceitos:
	* Domínio do problema: as fronteiras do que estamos tratando
	* Necessidades do negócio: o quê se quer atingir com o *software*, lembrando que o *software* não é o fim em si próprio. 
	* O *software*, depois de feito, deve atender às **necessidades do negócio** considerando o **domínio do problema** que o projeto pretende abarcar. No entanto, as **necessidades do negócio** não são requisitos do *software*
	* Restrições: são limitações que vão impactar o projeto
	* Regras de negócio: é como o negócio funciona, independentemente de *software*. Um exemplo: o cliente que já fez mais de 5 compras em uma loja é considerado cliente *premium*
* Requisitos de transição: representam uma etapa de transição entre o estado atual de solução do problema e o estado ao qual se deseja chegar com o projeto. Exemplos: 1) os dados da planilha eletrônica atualmente utilizada devem ser migrados de forma automática para o novo sistema; 2) o sistema atual e o novo sistema permanecerão em uso paralelo por duas semanas.
* Requisitos Funcionais: o quê o software precisa fazer
	* Um vendedor deve conseguir registrar uma venda sem realizar o cadastro do cliente
	* Um vendedor deve conseguir registrar uma venda indicando o cadastro do cliente através do CPF/CNPJ
	* Um professor deve conseguir lançar a presença dos alunos em cada aula
	* O sistema deve calcular a frequência dos alunos em uma disciplina de forma automática
	* **Atenção**: como as operações serão feitas no sistema (o passo a passo de como o usuário as irá fazer) não são requisitos do sistema!
* Requisitos Não funcionais: outras restrições que o software deve atender
	* Segurança, privacidade, etc.
	* Em que ambiente o sistema rodará
	* Quais padrões/protocolos o sistema seguirá
* Requisitos Inversos: expressam o quê o sistema não deve fazer. São importantes para boa definição do escopo e visam evitar ambiguidades
	* O sistema não deve arredondar os valores informados pelos usuários

"Alguns autores, como Ian Sommerville, também classificam requisitos em **requisitos de usuário** e **requisitos de sistema**. Requisitos de usuários são requisitos de mais alto nível, escritos por usuários, normalmente em linguagem natural e sem entrar em detalhes técnicos. Já requisitos de sistema são técnicos, precisos e escritos pelos próprios desenvolvedores. Normalmente, um requisito de usuário é expandido em um conjunto de requisitos de sistema. Suponha, por exemplo, um sistema bancário. Um requisito de usuário — especificado pelos funcionários do banco — pode ser o seguinte: "o sistema deve permitir transferências de valores para uma conta corrente de outro banco, por meio de TEDs". Esse requisito dá origem a um conjunto de requisitos de sistema, os quais vão detalhar e especificar o protocolo a ser usado para realização de tais transferências entre bancos. Portanto, requisitos de usuário estão mais próximos do problema, enquanto que requisitos de sistema estão mais próximos da solução." [1]
#### Referências bibliográficas
[1] https://engsoftmoderna.info/cap3.html
