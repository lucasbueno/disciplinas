## DNS: conceitos, importância, e aplicações

### Anotações do professor Lucas Bueno

##### Última atualização: 13/09/20199

- Há muito tempo, numa galáxia muito, muito distante… seres, talvez alienígenas, utilizavam um *software* chamado ICQ (“*I Seek You*”). O ICQ foi um dos pioneiros dos *softwares* de mensagens instantâneas na Internet, e ele tinha uma característica que talvez hoje fosse considerada como peculiar: no início, cada usuário era identificado unicamente através de um “número do ICQ”. Mas… quão fácil é memorizar um número de 5 dígitos? E de 8 dígitos?
  
  - Para saber mais: https://www.techtudo.com.br/listas/2019/06/icq-msn-sms-e-whatsapp-relembre-a-evolucao-de-mensagens-e-apps.ghtml
    
    Voltando para 2019:

- Aprendemos nas aulas anteriores, assim como na disciplina de Redes de Computadores, que o IP é o número que identifica um computador em uma rede de forma única;
  
  - Um exemplo de IP: 168.181.50.37

- Também aprendemos que é o servidor DHCP o responsável por atribuir endereços IPs para os *hosts* de forma automática

- Lembre-se: em nossas casas, por exemplo, normalmente temos apenas um único número IP na Internet, e que é o <u>roteador</u> o <u>computador</u> responsável por definir as rotas dos pacotes enviados da/para nossa rede interna, da/para a Internet, utilizando NAT (*Network Address Translation*, ou Tradução de Endereços de Rede);

- Mas quando queremos acessar um site, que endereço digitamos no nosso navegador?

- Chamamos o endereço que digitamos no navegador de “domínio” ou “nome de domínio”
  
  - No Brasil, o órgão responsável por registrar os nomes de domínio é o NIC.br (Núcleo de Informação e Coordenação do Ponto BR), o braço executivo do CGI.br (Comitê Gestor da Internet no Brasil), e você pode registrar seu domínio no https://registro.br

- Mas se digitamos um domínio no navegador, e os computadores são identificados unicamente através de um número de IP, como o domínio é convertido no número IP?

- Com um serviço chamado DNS (*Domain Name Server*, ou Serviço de Nomes de Domínio)

- O DNS é um **banco de dados distribuído**, funcionando com **sistemas cooperativos**, que trabalham de forma independente:
  
  - Sistemas cooperativos: trabalham em conjunto. Uma solicitação para tradução de um nome de domínio em um endereço IP feita a um servidor DNS, pode consultar também outros servidores DNS para entregar a resposta;
  - Banco de dados distribuído: as informações não são armazenadas em um único banco de dados central, elas estão distribuídas entre os vários bancos de dados. 

- O DNS pode ser classificado como para prover **serviços externos** para uma organização, como o acesso à Internet. Enquanto um servidor Samba, que implantamos nas aulas anteriores, para compartilhamento de arquivos, pode ser classificado como para prover serviços internos de uma organização;

- De maneira simplificada, o DNS funciona assim:
  
  - Um cliente, como um navegador, faz uma requisição para que um servidor DNS resolva um determinado domínio;
  - O servidor DNS faz a busca  até encontrar a entrada do domínio, ou não existirem mais possibilidades;
  - O servidor DNS retorna para o cliente ou o IP, ou um indicativo de erro.

- Antes de avançarmos, vale a pena definirmos a diferença entre o protocolo DNS e um serviço DNS:
  
  - O protocolo é a especificação, a documentação. É elaborado pela Internet Engineering Task Force (um grupo de trabalho internacional, em que os membros desenvolvem e promovem padrões para a Internet)
    - https://www.ietf.org/
    - Mais especificamente:
      - RFC 1034, DOMAIN NAMES - CONCEPTS AND FACILITIES
      - RFC 1035, DOMAIN NAMES -    IMPLEMENTATION AND SPECIFICATION
    - Enquanto um serviço DNS é a implantação, o *software* que segue o protocolo:
      - Nos mundos Unix e Linux, o Berkeley Internet Name Domain (BIND) é uma opção bastante popular;
      - No mundo Windows, o *software* de servidor DNS da Microsoft é também bastante popular;

- Toda esta história começou a ser desenvolvida já na década de 70, quando a Stanford Research Institue (SRI) era responsável pela ARPANET, e mantinha um arquivo de texto onde estavam mapeados cada domínio e seu respectivo endereço;
  
  - Como essa abordagem centralizada não era escalável, Paul Mockapetris criou na década de 80, com a ajuda de colegas como Jon Postel, o DNS.

- É importante citar que o DNS não serve apenas para tradução de domínios, mas também de servidores de e-mail e informações de outros servidores DNS;

- O DNS pode utilizar o protocolo TCP ou o UDP;

- Para realização da busca pela entrada de um domínio solicitada por um cliente:
  
  - É analisado o *Domain Namespace*, ou espaço de nomes do domínio, que é formado da seguinte maneira:
    - Considerando o domínio “https://mail.google.com”
      - o “.com” é chamado de domínio de *top level;*
      - o “.google” é chamado de domínio;
      - e o “mail” é chamado de subdomínio.
  - O primeiro servidor que será questionado sobre o domínio será um *recursive resolver*, que pode ser do seu provedor de Internet, de outro que você configurou, ou da sua organização
    - Este servidor saberá para qual outro servidor ele deve encaminhar a requisição;
  - O servidor *recursive resolver* enviará a requisição para um servidor raíz
    - Existem apenas 13 servidores raíz no mundo! Eles são gerenciados por grandes organizações.
    - Eles encaminham para os domínios de *top level* (.com, por exemplo)
  - O servidor de *top level* conhece os domínios daquele *top level*, (.google.com, por exemplo), e encaminha para o servidor DNS correto
  - A requisição é então encaminhada para o DNS, que conhece a resposta para o domínio completo, incluindo os subdomínios (mail.google.com, por exemplo)

- Muitas vezes utilizamos servidores de DNS externos, mas um servidor interno bem configurado, que faça *cache*, fará com que o processo seja mais eficiente, principalmente para a configuração de um servidor DNS para o domínio próprio das organizações;

- O processo de atualização dos *caches* dos servidores é chamado de propagação.
