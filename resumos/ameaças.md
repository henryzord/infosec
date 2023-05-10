# Tipos de Ameaças

## Sumário

* [Introdução](#introdução)
* [Malware](#malware)
* [Phishing](#phishing)
* [Man-in-the-Middle](#man-in-the-middle)
* [Denial-of-Service](#denial-of-service)

## Introdução

Existem diversas ameaças à Segurança da Informação, que visam atacar um ou mais dos seus pilares fundamentais, seja pela
exploração de vulnerabilidade em parcelas (software, hardware, ou comunicação), ou então em seus níveis (físico, 
pessoal, e organizacional). Esta seção trará alguns dos tipos de deliberados de ameaças à Segurança da Informação (ou 
seja, ameaças que não são decorrentes de falhas ou acidentes, mas sim perpetradas por terceiros mal-intencionados), e as 
melhores práticas do mercado no combate à elas.

## Malware

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

## Phishing

Phishing é um tipo de ataque que consiste em convencer uma primeira entidade (a vítima) de que a identidade de uma 
segunda (um golpista) é na verdade a de uma terceira (o “roubado”). O phishing ocorre exclusivamente entre entidades 
humanas (ou seja, nenhuma das entidades é um computador). Os tipos de dados furtados da pessoa roubada são geralmente de 
baixo potencial danoso, como a imagem do avatar em uma rede social, nome e sobrenome, idade, características pessoais 
como altura, peso, dentre outras. De posse dessa informações, o golpista tenta se passar por esta pessoa, de maneira a 
extrair informações mais relevantes da vítima. Para evitar ataques de phishing, organizações devem implementar 
autenticação, evitando que mensagens sejam trocadas por meios não seguros.

## Man-in-the-Middle

Um ataque do tipo man-in-the-middle (ou homem-no-meio, na tradução em português) é um em que um atacante possui acesso 
à troca de mensagens entre duas entidades, seja um cliente e um servidor, ou dois dispositivos de outra natureza em 
rede. De posse deste acesso, o atacante pode então incluir, modificar ou destruir informações, de maneira a causar 
contratempos à organização, ou mesmo roubar informações como credenciais de acesso. Para proteger-se deste tipo de 
ataque, é importante utilizar criptografia na troca de mensagens, bem como usar protocolos seguros como HTTPS e SSH.

## Denial-of-Service

Um ataque do tipo denial-of-service, ou negação de serviço, visa interromper o fluxo normal de troca de mensagens entre 
duas entidades. Entre um cliente e servidor, por exemplo, isto é obtido através do sobrecarragamento do número de 
requisições ao servidor, de maneira que este não possa respondê-las de maneira satisfatória. Caso obtenha sucesso, 
este ataque efetivamente interrompe o funcionamento normal da comunicação entre as entidades, o que pode acarretar em 
perdas financeiras. Também há a possibilidade que estes ataques sejam efetuados por uma organização de maneira a 
chantagear outra, ou causar perda de mercado. 

Prevenir ataques deste tipo pode ser uma tarefa difícil, dado que, a depender da natureza da aplicação, pode não ser 
trivial separar requisições legítimas de um ataque. Porém, o monitoramento de tráfego, e o uso de firewalls, são medidas 
que podem ser adotadas para mitigar o problema.