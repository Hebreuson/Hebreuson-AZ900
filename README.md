# Hebreuson-AZ900
Na aula de hoje aprendi um pouco mais sobre a plataforma do azure e estou motivado para o restante do aprendizado

Neste momento do cuso aprendi, sobre escabilidade e elasticidade, segurança em um modo geral e gerenciabilidade.
Um ponto muito importante é entender que cada recurso trabalha em conjunto um com o outro.

Na Aula de hoje aprendi as diferenças de IaaS, PaaS, Saas.
No entanto segue o aprendizado:
IaaS se refere a Infraestrutura como serviço;
PaaS se refere a Plataforma como serviço;
SaaS se refere a Software como serviço;
On Primise se refere quando a empresa detem todo o parque de TI fisicamente na empresa. 

Foi apresentado tambem, os modelos de gerenciamento, mostrando a tabela de modelo de responsabilidade, sendo elas:
Iaas tendo a maior gestão;
Paas tendo uma gestão intermediaria;
SaaS tendo a menor gestão;

Lembrando que a gestão se refere sempre ao Cliente, e os serviços da microsoft podem ser adicionados ou não, sendo uma escolha do TI.

Na primeira aula do modolo 2 do curso foi apresentado a aquitetura da microsoft Azure.
Na qual é formada por diversas regiões de disponibilidade, contendo grupos de gerenciamento, assinaturas, grupos de recursos e recursos.
Sendo primordial entender que cada região tem sua disponibilidade par, quando uma região ococorre um desastre recovery, sempre tera outra região para suprir a necessidade da demanda afetada.
Importante lembrar que se a impresa não adquire este recurso de disponibilidade, ela fica refém de ter que esperar o sistema retornar a funcionar, impactando a redundancia do projeto. 
É muito importante salientar que uma conta pode ter diversas assinaturas e recursos, mas não podemos ter assinaturas em diversas contas diferentes, todas devem responder por apenas uma conta gerenciada da microsoft Azure. 

Ate o momento foi aprendido sobre as functions da microsoft azure, e suas redes, conterners e suas disponibilidades.
Em um resumo, podemos criar diversas diversas redudancias em nosso sistema em nuvem, sendo gerado por 1 ou mais disponibilidades, como por exemplo, temos 3 dispositivos com o mesmo recurso de arquivos, pacote de dados e aplicativos sendo executados simultaneamente, caso ocorra algum desatre Em um Rack que contem a VM do produto sendo executado, o mesmo vai rodar na disponibilidade 2, caso a disponibilidade 2 cair o sistema, vai para a disponibilidade 3, sendo gerado sempre uma redundancia no sistema.
Isto esta ligado mais a um IaaS, porem quando estamos falando de apenas recursos de aplicativos e sirviços sendo rodados, estamos falando de PaaS. 

Aprendemos tambem sobre os Contêiners, que utiliza uma função rapida para diversas soluções de problemas, em resumo podemos criar um conteiner com diversos conteiners dentro dele, sendo facil o gerenciamento e exclução posteriormente.
Já falando em redes, o cliente pode solicitar uma conexão direta via VPN em nuvem que conecta na Azure para o on-primese, mas podemos também conectar o express route, aonde tem uma conexão mais rapida e "segura" que somente a conexão vpn diramante em nuvem a VNET, conexão virtualizada da nuvem. 
A conexão express route, é realizada por uma empresa credenciada pela microsoft, que vai gerenciar uma conexão via fibra opicta direta com a microsoft, deixando o sistema mais rapido e privado. 
De um modo geral a Microsoft Azure faz um gerenciamento em DNS, dando um nome para cada função e registro; Sendo necessário ter um ip diferente um do outro. 

Hoje o dia foi muito produtivo ate o momento, realizei uma criação de uma maquina virtual no Azure, realizei uma criação de recursos e de uma vnet, verifiquei o que é uma area de trabalho virtual Azure e funções.
Nas proximas aulas irei aprender sobre armazenamento. 

Hoje aprendi sobre Armazenamento Azure, as contas de armazenamento devem ter um nome exclusivo.
e devem ter opções de redundacias.

LRS: ARMAZENAMENTO COM REDUNNCIA: DATA CENTER INDIVUDUAL 11 noves (caso o datacenter caia o sistema é perdido)

ZRS: ARMAZENAMENTO COM REDUNDANCIA DE ZONA 12 noves (tres zonas de disponibilidade na região primaria) (caso o datacenter caia ele tera mais 2 copias para subir o sistema, só fica sem se a região inteira cair. 

GRS: ARMAZENAMENTO COM REDUNCIA GEOGRAFICA 16 noves (datacenter unico primairo e regiao secundaria) (caso o servidor caia na região primaira ele tera um par na regiao secundaria)

GZRS: ARMAZENAMENTO COM REDUNDANCIA DE ZONA GEOGRAFICA 16 noves (tres zonas de disponibilidade na regiao primaria e um unico datacenter na regiao secundaria) (caso o data center caia na região ele tera uma copia em outra região par)

