# Segurança da Informação

## Sumário

* [Introdução](#Introdução)
* [Princípios da Segurança da Informação](#Princípios-da-segurança-da-Informação)
    * [Pilares fundamentais](#Pilares-fundamentais)
    * [Parcelas da Segurança da Informação](#Parcelas-da-Segurança-da-Informação)
    * [Níveis da Segurança da Informação](#Níveis-da-Segurança-da-Informação)
* [Tipos de Ameaças](#Tipos-de-Ameaças)
    * [Malware](#Malware)
    * [Phishing](#Phishing)
    * [Man-in-the-Middle](#Man-in-the-Middle)
    * [Denial-of-Service](#Denial-of-Service)
* [Medidas de Segurança](#Medidas-de-Segurança)
    * [Controle de Acesso](#Controle-de-Acesso)
    * [Firewalls](#Firewalls)
    * [Encriptação](#Encriptação)
    * [Backup e recuperação](#Backup-e-recuperação)
* [Conclusão](#Conclusão)

## Introdução

A segurança da informação é a área da Ciência da Computação que preocupa-se com manter dados protegidos do uso 
não-autorizado por terceiros, para propósitos como uso, divulgação, modificação, ou destruição. Com a popularização da 
Internet e meios digitais de comunicação, esta área tem ganhado importância, sendo aplicada desde aplicativos de troca 
de mensagens como o Whatsapp, passando por hospitais que armazenam dados médicos de seus pacientes, até organizações 
financeiras como o Banco Central, que busca manter a integridade das transações digitais com o advento do PIX. O não-uso
 de conceitos da Segurança da Informação poderia permitir que pessoas não autorizadas observem mensagens que são 
 destinadas à terceiros, acessem registros médicos, e falsifiquem transações bancárias, nos exemplos citados acima.

A Segurança de Informação baseia-se em três pilares: garantir a confidencialidade, disponibilidade e integridade de 
informações. Ela também preocupa-se em garantir a autenticidade e não-repudiação da troca de informações (i.e. 
certificar que dois entes de fato se comunicaram, e que esta troca não pode ser falsificada).

Confidencialidade diz respeito à preservação da privacidade das mensagens, prevenindo acesso, uso ou conhecimento por 
pessoas ou entidades não-autorizadas. A confidencialidade pode ser obtida através da criptografia, e controle de acesso 
através da autenticação à aplicativos de troca de mensagem. Já a disponibilidade diz respeito a possibilidade de 
usuários autorizados acessarem informações no momento em que esses assim desejarem, sem interrupções ou interferências. 
Finalmente, a integridade de informações garante que as mesmas não foram modificadas, corrompidas, ou destruídas, de 
maneira acidental ou proposital. A integridade de dados é garantida através da criptografia, controle de acesso, e 
backups. 

É importante salientar que a Segurança da Informação não opera apenas no nível de hardware e/ou hardware, mas também no 
nível organizacional. Em outras palavras, não basta manter equipamentos fisicamente seguros, nem softwares atrás de 
telas de login, quando a cultura da organização (seja uma empresa, universidade ou outra entidade) não estiver voltada 
à segurança também. Em uma organização que não prioriza a segurança, por exemplo, é possível que uma pessoa 
não-credenciada acesse espaços privados através de engenharia social, como por exemplo acessar portas controladas por 
cartão de acesso, ou então acessar computadores que não estão protegidos com senha, e foram deixados sem supervisão por 
um funcionário ou pessoa que se ausentou para ir ao banheiro, por exemplo.

Dado que a Segurança da Informação possui muitos tópicos, cada um com suas particularidades, este texto visa cobrir de 
maneira breve, porém abrangente, cada um dos assuntos pertinentes à Segurança da Informação, de maneira a apresentar o 
leitor com um panorama conciso desta área do conhecimento.

O resto do texto é organizado da seguinte maneira. A Seção 
[Princípios da Segurança da Informação](#Princípios-da-segurança-da-Informação) abordará em maiores detalhes cada um dos 
três pilares da Segurança da Informação, enquanto a Seção [Tipos de Ameaças](#Tipos-de-Ameaças) detalhará os tipos de 
ameaças presentes à estes pilares. A Seção [Medidas de Segurança](#Medidas-de-Segurança) traz técnicas e princípios 
adotados para mitigar estas ameaças, enquanto a Seção [Conclusão](#Conclusão) conclui o texto e traz direções futuras 
para esta área do conhecimento.

## Princípios da Segurança da Informação

A segurança da informação é dividida entre três pilares fundamentais: confidencialidade, disponibilidade, e integridade. 
Estes três pilares são aplicados em três parcelas, hardware, software, e comunicações, e em três níveis (ou camadas); 
física, pessoal e organizacional.

### Pilares fundamentais

Os pilares fundamentais da Segurança da Informação, também chamados de qualidades, são a confidencialidade, 
disponibilidade, e integridade. São ditos qualidades pois é preferível que as informações possuam estas características 
dentro de uma organização. 

A confidencialidade de informações garante que elas não serão acessadas por entes terceiros, não autorizados, seja 
acidentalmente ou intencionalmente. Estes entes terceiros podem ser pessoas, algoritmos ou computadores. Garantir a 
confidencialidade é importante para diversas aplicações, como manutenção de registros médicos, dados financeiros, 
histórico de localização de usuários, dentre outros. A manutenção da confidencialidade permite que usuários de um 
sistema construam uma relação de confiança com o mesmo. A quebra de confidencialidade pode acarretar em consequências 
como venda ilegal de informações no mercado negro, chantagem (inclusive na forma de vírus de computador, chamados 
randomwares), perda de vantagem comercial (quando tratando-se de informações sobre uma empresa), dentre outros. Uma
maneira de garantir a confidencialidade é a aplicação de controle de acesso às informações, bem como a criptografia.
A disponibilidade garante que as informações estarão disponíveis no momento em que forem necessárias, ou que a 
comunicação entre dois entes seja possível assim que necessária. Existem ataques voltados à negação da disponibilidade, 
como o Denial-of-Service, que será abordado em maiores detalhes na Seção 6.2.4. A interrupção da disponibilidade pode 
acarretar desde transtornos para usuários individuais, quanto perda de dinheiro para empresas ou negócios, visto que 
estas não podem executar normalmente seu trabalho. Garante-se a disponibilidade de informações através de redundância, 
como manter cópias de registros em diversos servidores. Isto reduz as chances de que um ataque seja bem-sucedido na 
negação de serviços, por exemplo, por aumentar o custo do ataque (mais servidores para atacar).

Finalmente, a integridade de informações garante que estas não foram modificadas ou destruídas, intencionalmente ou 
acidentalmente, por entes terceiros ou outros fenômenos (e.g. quedas de energia). A integridade é garantida através do 
controle de acesso às informações, e redundância, ao manter-se registros em mais de um servidor ou computador, por 
exemplo. Uma não-observância da integridade de informações pode acarretar em perdas econômicas, visto que registros 
podem ser perdidos (por estarem corrompidos), ou até mesmo serem alterados para demonstrar informações incorretas. 

### Parcelas da Segurança da Informação

A segurança da informação é dividida em três parcelas: hardware, software, e comunicação. Estas três parcelas funcionam 
em conjunto, simultaneamente, e é preciso garantir a segurança nelas a todo o momento. Por exemplo, em um aplicativo de 
troca de mensagens como o Whatsapp, duas pessoas estão se comunicando através de um software, o aplicativo, que é 
executado em diversos hardwares (os dois celulares, mais todos os equipamentos conectados em rede que permitem a 
comunicação entre estes dois aparelhos). Uma não-garantia da segurança da informação em qualquer uma destas parcelas 
colocará em risco as mensagens que estão sendo trocadas.

Garantir a Segurança de Informação do hardware envolve medidas tanto a nível físico, de manutenção do equipamento em 
local fechado, quanto de software. Ao restringir o acesso físico ao hardware, como por exemplo colocá-lo em uma sala 
com controle de acesso, diminui-se a possibilidade de que pessoas irão mexer neste hardware em busca de vulnerabilidades
(e.g. abrindo-o, colocando pendrives que executam código malicioso, etc). Já a segurança à nível de hardware inclui por 
exemplo configurar uma senha para que o computador possa passar pelo boot, evitando que alguém não-autorizado apague as 
informações ao formatar a máquina; e atualizá-lo para usar os softwares mais recentes de aplicações e sistema 
operacional, que incluem correções à vulnerabilidades encontradas em versões anteriores.

A segurança a nível de software é montada a partir de diversas medidas técnicas e não-técnicas. Como medidas técnicas, 
podemos citar o emprego de boas práticas de programação, visando minimizar vulnerabilidades com SQL injection; testes 
de segurança, visando encontrar vulnerabilidades no sistema; atualizações constantes aos softwares envolvidos; dentre 
outros. Como medidas não-técnicas, está o controle de acesso a repositórios de código-fonte por pessoas não autorizadas; 
monitoramento e logging, mantendo registros de quem acessou quais recursos computacionais a qual tempo; e planejamento 
de recuperação de desastres, tendo assim um plano de contigência para caso catástrofes ocorram.

Finalmente, a segurança à nível de comunicação diz respeito a garantir que a troca de informações entre duas ou mais 
entidades tenha as três qualidades da Segurança da Informação. Medidas para garantir a segurança nesta parcela incluem: 
a criptografia de mensagens, impedindo que terceiros compreendam as informações trocadas; uso de protocolos de 
comunicação seguros, como HTTPS, SSH, dentre outros, garantindo a proteção contra escuta e modificação dos dados 
transmitidos; uso de firewalls, que filtram mensagens com potencial danoso de serem transmitidas por uma rede; dentre 
outras medidas.

### Níveis da Segurança da Informação

A Segurança da Informação possui três níveis: físico, pessoal e organizacional. Da mesma maneira como as parcelas, os 
três níveis operam ao mesmo tempo, sendo necessário garantir a segurança dos três níveis simultaneamente para obter-se 
um ambiente seguro.

A segurança física diz respeito aos aspectos físicos do ambiente onde informaçẽos transitam, como escritórios, racks de 
servidores, espaços compartilhados, dentre outros.

## Tipos de Ameaças 

Existem diversas ameaças à Segurança da Informação, que visam atacar um ou mais dos seus pilares fundamentais, seja pela
exploração de vulnerabilidade em parcelas (software, hardware, ou comunicação), ou então em seus níveis (físico, 
pessoal, e organizacional). Esta seção trará alguns dos tipos de deliberados de ameaças à Segurança da Informação (ou 
seja, ameaças que não são decorrentes de falhas ou acidentes, mas sim perpetradas por terceiros mal-intencionados), e as 
melhores práticas do mercado no combate à elas.

### Malware

Um malware (termo reduzido de “malicious software”, ou software malicioso) é definido como um software que tem com o 
objetivos ganhar acesso não-autorizado à aplicações, destruir informações, ou interromper o fluxo de dados entre duas 
entidades. Malware é um termo abrangente que inclui diversos tipos de software, como vírus de computador, worms, 
trojans, ransomwares, dentre outros. 

Existem diversas maneiras de se proteger contra malwares, sendo algumas: manter os softwares utilizados atualizados, 
integrando correções à vulnerabilidades encontradas em versões anteriores; o uso de firewalls, que monitoram as 
informações trocadas entre entidades em uma rede de computadores, e detém o poder de recusar certas trocas de 
informações caso uma ameaça seja detectada; redundância no armazenamento de informações, como guardar os mesmos dados 
em mais de um servidor, evitando assim que uma perda catastrófica em um servidor acarrete na perda total de dados da 
organização; e uso de anti-vírus, que escaneiam arquivos de um computador em busca de anormalidades (e.g. arquivos que 
possuem uma assinatura digital diferente da esperada).

### Phishing

Phishing é um tipo de ataque que consiste em convencer uma primeira entidade (a vítima) de que a identidade de uma 
segunda (um golpista) é na verdade a de uma terceira (o “roubado”). O phishing ocorre exclusivamente entre entidades 
humanas (ou seja, nenhuma das entidades é um computador). Os tipos de dados furtados da pessoa roubada são geralmente de 
baixo potencial danoso, como a imagem do avatar em uma rede social, nome e sobrenome, idade, características pessoais 
como altura, peso, dentre outras. De posse dessa informações, o golpista tenta se passar por esta pessoa, de maneira a 
extrair informações mais relevantes da vítima. Para evitar ataques de phishing, organizações devem implementar 
autenticação, evitando que mensagens sejam trocadas por meios não seguros.

### Man-in-the-Middle

Um ataque do tipo man-in-the-middle (ou homem-no-meio, na tradução em português) é um em que um atacante possui acesso 
à troca de mensagens entre duas entidades, seja um cliente e um servidor, ou dois dispositivos de outra natureza em 
rede. De posse deste acesso, o atacante pode então incluir, modificar ou destruir informações, de maneira a causar 
contratempos à organização, ou mesmo roubar informações como credenciais de acesso. Para proteger-se deste tipo de 
ataque, é importante utilizar criptografia na troca de mensagens, bem como usar protocolos seguros como HTTPS e SSH.

### Denial-of-Service

Um ataque do tipo denial-of-service, ou negação de serviço, visa interromper o fluxo normal de troca de mensagens entre 
duas entidades. Entre um cliente e servidor, por exemplo, isto é obtido através do sobrecarragamento do número de 
requisições ao servidor, de maneira que este não possa respondê-las de maneira satisfatória. Caso obtenha sucesso, 
este ataque efetivamente interrompe o funcionamento normal da comunicação entre as entidades, o que pode acarretar em 
perdas financeiras. Também há a possibilidade que estes ataques sejam efetuados por uma organização de maneira a 
chantagear outra, ou causar perda de mercado. 

Prevenir ataques deste tipo pode ser uma tarefa difícil, dado que, a depender da natureza da aplicação, pode não ser 
trivial separar requisições legítimas de um ataque. Porém, o monitoramento de tráfego, e o uso de firewalls, são medidas 
que podem ser adotadas para mitigar o problema.

## Medidas de Segurança

Esta seção discorre de maneira mais detalhada sobre cada uma das medidas de segurança que podem ser tomadas para 
garantir a Segurança de Informação em organizações.

### Controle de Acesso

Controlar o acesso de pessoas à espaços físicos, bem como à softwares, é uma medida básica para qualquer organização que 
queira ter um mínimo de segurança; do contrário, qualquer pessoa (ou software) pode acessar informações prontamente 
disponíveis, seja na Internet, ou nos espaços físicos. No nível físico, o controle de acesso pode ser implementado com 
cartões de acesso, enquanto no nível pessoal credenciais (usuário e senha) podem ser usados para regular o acesso à 
computadores, redes e softwares.

### Firewalls

Firewalls são um tipo de software, executado em um roteador de rede, que faz a filtragem de pacotes que são trocados 
entre dispositivos conectados através do roteador. Um firewall então bloquear mensagens com potencial danoso, através da 
identificação do seu conteúdo. 

### Encriptação

A encriptação aplica-se à mensagens que são trocadas entre duas entidades, impossibilitando que uma terceira entidade, 
por mais que obtenha acesso ao conteúdo das mensagens, consiga fazer um uso inteligível dela. Com isto, mesmo um acesso 
não-autorizado à uma rede não acarreta na adulteração ou uso indevido de mensagens. A encriptação é obtida ao 
utilizar-se algoritmos de criptografia nas mensagens, bem como utilizar protocolos seguros de troca de mensagens como 
SSH e HTTPS.

### Backup e recuperação

O backup de dados faz uma ou mais cópias de determinado conjunto de dados, e preferencialmente armazena estas cópias em 
outro ou outros dispositivos, que não o que gerou os dados originais. Desta maneira, mesmo que um dispositivo fique 
inoperante, seja qual for o motivo, os dados estarão disponíveis em outro dispositivo. É importante manter o mesmo nível 
de segurança à estes dados de backup conferido aos dados originais, através de criptografia e controle de acesso.

## Conclusão

A Segurança da Informação é uma importante área do conhecimento, que visa proteger dados, troca de mensagens e 
informações, seja no nível pessoal, ou (e principalmente) organizacional. Através da aplicação de diversas técnicas em 
diferentes parcelas (software, hardware, e comunicações), e em diferentes níveis (física, pessoal e organizacional), 
garante-se os três pilares fundamentais da Segurança da Informação: confidencialidade, disponibilidade e integridade.

A Segurança da Informação é uma área em constante desenvolvimento, realizando pesquisas em novas tecnologias para 
manter-se à par de agentes que buscam miná-la. Como exemplo de novas pesquisas na área, pode-se citar: o uso de 
algoritmos de Aprendizado de Máquina na identificação de pacotes que transitam em firewalls; a pesquisa de novos 
algoritmos de criptografia, resistente ao uso de computadores quânticos, que podem tornar os algoritmos de criptografia 
antigos obsoletos; dentre outros desenvolvimentos.
