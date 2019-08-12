ChatContent

Essa classe cont�m a vari�vel listSectionConversa e os m�todos ChatContent, isSameSection e getLastMensagemWa.

Assinatura

public ChatContent(List<MensagemWhatsapp__c> pListMensagemWa)

Explecifica��es

@AuraEnabled
listSectionConversa

Cria a vari�vel p�blica do tipo lista de SectionConversa.

Assinatura

public List<SectionConversa> listSectionConversa;

ChatContent(pListMensagemWa)

Atribui os valores da vari�vel p�blica listSectionConversa atrav�s da lista de mensagens passada pelo par�metro pListMensagemWa.

Assinatura

public ChatContent(List<MensagemWhatsapp__c> pListMensagemWa)

Valor retornado

Sem retorno.


isSameSection(pSectionConversa, pMensagemWa)

Verifica se a �ltima mensagem da pSectionConversa � igual � mensagem enviada via par�metro pMensagemWa, retornando true caso for verdade e false caso contr�rio.

Assinatura

public Boolean isSameSection(SectionConversa pSectionConversa, MensagemWhatsapp__c pMensagemWa)

Valor retornado

Tipo:	Boolean.

getLastMensagemWa(pSectionConversa)

Retorna a �ltima mensagem do par�metro enviado pSectionConversa.

Assinatura

public MensagemWhatsapp__c getLastMensagemWa(SectionConversa pSectionConversa)

Valor retornado

Tipo:	MensagemWhatsapp__c.
