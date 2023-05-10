# Segurança da Informação

## Sumário

* [Introdução](#Introdução)
* [Princípios da Segurança da Informação](princípios.md)
    * [Pilares fundamentais](princípios.md#pilares-fundamentais)
    * [Parcelas da Segurança da Informação](princípios.md#parcelas-da-segurança-da-informação)
    * [Níveis da Segurança da Informação](princípios.md#níveis-da-segurança-da-informação)
* [Tipos de Ameaças](ameaças.md)
    * [Malware](ameaças.md#malware)
    * [Phishing](ameaças.md#phishing)
    * [Man-in-the-Middle](ameaças.md#man-in-the-middle)
    * [Denial-of-Service](ameaças.md#denial-of-service)
* [Medidas de Segurança](medidas_de_segurança.md)
    * [Controle de Acesso](medidas_de_segurança.md#controle-de-acesso)
    * [Firewalls](medidas_de_segurança.md#firewalls)
    * [Encriptação](medidas_de_segurança.md#encriptação)
    * [Backup e recuperação](medidas_de_segurança.md#backup-e-recuperação)
* [Futuro da Segurança da Informação](futuro.md)

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
[Princípios da Segurança da Informação](princípios.md) abordará em maiores detalhes cada um dos 
três pilares da Segurança da Informação, enquanto a Seção [Tipos de Ameaças](ameaças.md) detalhará os tipos de 
ameaças presentes à estes pilares. A Seção [Medidas de Segurança](medidas_de_segurança.md) traz técnicas e princípios 
adotados para mitigar estas ameaças, enquanto a Seção [Futuro da Segurança da Informação](#futuro.md) traz direções futuras 
para esta área do conhecimento.
