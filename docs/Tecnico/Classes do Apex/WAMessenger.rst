WAMessenger_ctl

conversaWhatsappId

Get e Set da vari�vel p�blica do tipo String.

Assinatura

public String conversaWhatsappId {get;set;}

Valor retornado

Tipo de retorno do get:		String.
Tipo do retorno do set:		sem retorno.

conversaWa

Get e Set da vari�vel p�blica do tipo ConversaWhatsapp__c.

Assinatura

public ConversaWhatsapp__c conversaWa {get;set;}

Valor retornado

Tipo de retorno do get:		ConversaWhatsapp__c.
Tipo do retorno do set:		sem retorno.

msg

Get e Set da vari�vel p�blica do tipo String.

Assinatura

public String msg {get;set;}

Valor retornado

Tipo de retorno do get:		String.
Tipo do retorno do set:		sem retorno.

refreshPeriod

Get e Set da vari�vel p�blica do tipo Decimal.

Assinatura

public Decimal refreshPeriod {get;set;}

Valor retornado

Tipo de retorno do get:		Decimal.
Tipo do retorno do set:		sem retorno.

WAMessenger_ctl()

Atribui o valor para a v�riavel p�blica refreshPeriod.

Assinatura

public WAMessenger_ctl()

Valor retornado

Sem retorno.

getIconId()

Retorna a URL do �cone do Contato do Whatsapp relacionado a Conversa do Whatsapp atribu�da � vari�vel p�blica conversaWA.

Assinatura

public String getIconId()

Valor retornado

Tipo:	String.

resetData()

Atribui null � vari�vel local conversaWA.

Assinatura

public void resetData()

Valor retornado

Sem retorno.

getConversaWhatsapp()

Retorna a Conversa do Whatsapp do Id igual � vari�vel p�blica local conversaWhatsappId.

Assinatura

public ConversaWhatsapp__c getConversaWhatsapp()

Valor retornado

Tipo:	ConversaWhatsapp__c.

saveMessage()

Insere uma nova mensagem no servidor, atrav�s das vari�veis p�blicas locais msg e conversaWA.

Assinatura

public void saveMessage()

Valor retornado

Sem retorno.

@AuraEnabled
getConversaWa(pConversaWaId)

Retorna a Conversa do Whatsapp do Id igual � vari�vel p�blica local conversaWhatsappId.

Assinatura

public static ConversaWhatsapp__c getConversaWa(String pConversaWaId)

Valor retornado

Tipo:	ConversaWhatsapp__c.

@RemoteAction
getMensagemWa(pConversaWaId)

Retorna as �ltimas 1000 Mensagem do Whatsapp relacionado ao Id do par�metro passado  pConversaWaId.

Assinatura

global static List<MensagemWhatsapp__c> getMensagemWa(String pConversaWaId)

Valor retornado

Tipo:	List<MensagemWhatsapp__c>.


@AuraEnabled
getChatContent(pConversaWaId)

Retorna uma classe ChatContent, enviando as �ltimas 1000 mensagens da conversa com o Id igual � pConversaWaId como par�metro.

Assinatura

public static ChatContent getChatContent(String pConversaWaId)

Valor retornado

Tipo:	ChatContent.


@AuraEnabled
doSaveMessage(pConversaWhatsapp, pCorpo)

Insere uma nova mensagem no servidor, com os par�metros enviados pCorpo e pConversaWhatsapp.

Assinatura

public static void doSaveMessage(ConversaWhatsapp__c pConversaWhatsapp, String pCorpo)

Valor retornado

Sem retorno.

@AuraEnabled
getIconUrl(pContatoId)

Retorna a URL do icone do Contato do Whatsapp com o id pContatoId n�o tenha icone e retorna uma String vazia caso contr�rio.

Assinatura

public static String getIconUrl(String pContatoId)

Valor retornado

Tipo:	String.



getHostUrl()

Retorna a URL da organiza��o.

Assinatura

public static String getHostUrl()

Valor retornado

Tipo:	String.

@AuraEnabled
getWAActions(pConversaWhatsapp)

Retorna uma lista AcaoMessenger com os tipos de metadados de A��o do Whatsapp do tipo Messenger com a pConversaWhatsapp.

Assinatura

public static List<AcaoMessenger> getWAActions(ConversaWhatsapp__c pConversaWhatsapp)

Valor retornado

Tipo:	List<AcaoMessenger>.

@AuraEnabled
doExecuteAction(pAcaoWhatsapp, pConversaWhatsapp)

Executa o m�todo doExecuteWaAction da classe WAActionHandler.

Assinatura

public static void doExecuteAction(AcaoWhatsapp__mdt pAcaoWhatsapp, ConversaWhatsapp__c pConversaWhatsapp)

Valor retornado

Sem retorno.


