# Princípios da Segurança da Informação

## Sumário

* [Introdução](#introdução)
* [Pilares fundamentais](#pilares-fundamentais)
* [Parcelas da Segurança da Informação](#parcelas-da-segurança-da-informação)
* [Níveis da Segurança da Informação](#níveis-da-segurança-da-informação)

## Introdução

A segurança da informação é dividida entre três pilares fundamentais: confidencialidade, disponibilidade, e integridade. 
Estes três pilares são aplicados em três parcelas, hardware, software, e comunicações, e em três níveis (ou camadas); 
física, pessoal e organizacional.

## Pilares fundamentais

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

## Parcelas da Segurança da Informação

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

## Níveis da Segurança da Informação

A Segurança da Informação possui três níveis: físico, pessoal e organizacional. Da mesma maneira como as parcelas, os 
três níveis operam ao mesmo tempo, sendo necessário garantir a segurança dos três níveis simultaneamente para obter-se 
um ambiente seguro.

A segurança física diz respeito aos aspectos físicos do ambiente onde informaçẽos transitam, como escritórios, racks de 
servidores, espaços compartilhados, dentre outros.