# Gestão de Tecnologia da Informação

## Anotações do professor Lucas Bueno

### Última atualização: 04/02/2021

#### Segurança da informação: introdução
- “Segurança não é um produto, mas um processo” -- Bruce Schneier;
- A informação é um dos nossos bens mais preciosos;
- Podemos pensar a Segurança da Informção (SI) sem falar de computadores. No entanto, hoje, a maior parte da informação é controlada por computadores. Sendo assim, trabalharemos neste contexto;
- A segurança da informação foi muito relevante no século XX, principalmente nas guerras -- em especial com a quebra da máquina alemã Enigma (ver "O Jogo da Imitação");
- Durante a guerra fria o uso de computadores se intensificou e se criou a ARPANET. Neste momento, os estudiosos em segurança da informação passaram a dedicar grandes esforços para proteger também os acessos remotos;
- A partir de 1980 o uso de computadores pessoais passou a aumentar e, principalmente a partir de 1990, com a Internet, também a importância da SI;
- A crescente adoção do dispositivos IOT --- com o Amazon Echo, o Google Nest e sistemas para monitoramento residencial, também aumenta a preocupação com SI;


#### Segurança da informação: alguns conceitos
 - "A Segurança em TI é como trancar sua casa ou seu carro – não vai impedir os bandidos, mas se a tranca for boa o bastante, eles podem preferir buscar um alvo mais fácil." -- Paul Herbka;
 - Qualquer coisa que tenha valor para uma empresa é chamado de **ativo**. Assim, podemos dizer que um ativo de informação é o conjunto de informações que tem valor para a empresa;
 - As **vulnerabilidades** são fatores internos capazes de expor as informações de um sistema ao furto, roubo, perda, corrupção ou uso indevido. São pontos fracos que devem ser identificados e eliminados do ambiente empresarial.
   - As **vulnerabilidades ambientais** são aquelas relacionadas ao meio ambiente e à geografia do local onde a infraestrutura de tecnologia da informação da empresa está instalada;
   - As **vulnerabilidades de infraestrutura** são aquelas restritas ao ambiente que abriga a infraestrutura de tecnologia da informação da empresa, bem como os locais por onde a informação trafega;
   - As **vulnerabilidades de armazenamento** são aquelas relacionadas aos meios físicos, também conhecidos como mí dias, onde a informação está armazenada;
   - As **vulnerabilidades de transmissão** são aquelas relacionadas aos aspectos da comunicação de dados, abrangendo os meios físicos de transmissão (cabeamento, ondas de rádio, microondas, etc.) e os meios onde estes estão assentados (postes, tubulações, etc.);
   - As **vulnerabilidades de _hardware_** são aquelas relacionadas aos equipamentos, vistos de modo individual;
   - As **vulnerabilidades de _software_** são aquelas relacionadas às falhas de desenvolvimento e implantação dos aplicativos, sistemas operacionais e protocolos de comunicação;
   - As **vulnerabilidades humanas** são aquelas decorrentes da ação ou omissão dos seres humanos.
 - Já os **princípios** da SI são conceitos gerais que orientam a atividade de segurança. São eles:
   - Confidencialidade: estabelece que somente pessoas previamente autorizadas tenham conhecimento do conteúdo da informação;
   - Integridade: estabelece que a informação só pode sofrer reduções, acréscimos ou atualizações por pessoas previamente autorizadas, o que mantém suas características originais e respeita seu ciclo de vida;
   - Disponibilidade: estabelece que a informação deve estar sempre acessível às pessoas previamente autorizadas, no momento em que necessitam utilizá-la;
   - Autenticidade: estabelece que as informações, transações e comunicações devem ter uma origem comprovada, autores e/ ou operadores identificados, e não terem sido alvo de alterações imprevistas;
   - Irretratabilidade: estabelece que pessoas identificadas e autenticadas em um sistema de informações não possam repudiar terem criado ou alterado dados contidos em informações, transações ou comunicações;
 - Enquanto os **problemas** enfrentandos pela SI podem ser classificados em:
   - _Malwares_ (_software_ malicioso): programa de computador que se aproveitam de falhas de outros programas e que tem por objetivo provocar a perda de informações, utilizar indevidamente informações ou controlar remotamente um computador. Os principais tipos de _malwares_ são:
     - vírus: infectam um sistema e espalham cópias deles mesmos em outros programas/arquivos;
     - cavalos de troia (_trojans_): programas aparentemente seguros, mas que abrem uma porta de entrada para que seu computador possa ser controlado remotamente;
     - _spywares_: programas aparentemente seguros, mas com a inteção de coletar informações do usuário e enviá-las para um servidor;
     - _ransonwares_: programa que visa o sequestro de dados dos usuários, i.e., bloqueia o acesso aos dados e pede uma quantia em $$ para devolvê-los (como o famoso WannaCry);
     - _worms_: programas que não exigem a intervenção do usuário, principalmente por infectarem sistemas operacionais ou protocolos de rede. Sendo assim, eles se espalham muito rapidamente.
 - Enquanto exemplos de **soluções** para evitarmos as **vulnerabilidades** e atingirmos os **princípios** são:
   - **Gerenciadores de senha**: com a enorme quantidade de serviços protegidos por senha, não é ideal que utilizemos a mesma senha em todos eles (se um serviço for hackeado e sua senha for descoberta, a dos outros também é automaticamente descoberta) e nem que as anotemos em quaisquer lugares;
     - Ex.: Password Safe.
   - **Gerenciadores de backups**: nos auxiliam a criar cópias de segurança, idealmente de forma automática e "desconectado" da origem dos dados;
     - Ex.: SyncBackup.
   - **Ferramentas de criptografia**: possibiltam criptografar os dados e garantir que os mesmos só sejam acessados através de identificação e senha;
     - Ex.: TrueCrypt.
   - **Ferramentas para descarte de dados**: dificultam a recuperação dos dados de um HD, pois quando excluimos um arquivo o sistema operacional apenas remove os índices que informavam que naquela região havia um arquivo;
     - Ex.: Eraser.
   - **Ferramentas antivírus**: previnem, detectam e removem vírus de computadores. Idealmente devem estar sempre atualizados e rodando continuamente;
     - Ex.: Avast!.
   - **Ferramentas de _antispyware_**: similares aos antivírus, mas com foco em _spywares_;
     - Ex.: Spybot Search & Destroy.
   - **_Firewalls_**: avaliam e permitem ou bloqueiam o tráfego de determinados pacotes na rede ou de/para um computador;
     - Ex.: Comodo.
   - O **usuário**: "Nós, os profissionais de segurança, somos muito parecidos com médicos cardiologistas." -- Gene Spafford.
#### Referências bibliográficas
1. Softwares de segurança da informação / Jorge Procópio da Costa Novo. - Manaus : Centro de Educação Tecnológica do Amazonas ; Florianópolis : UFSC, 2010.
