param

Get e Set da vari�vel p�blica do tipo ParametroWahtsapp__c.

Assinatura

public ParametroWhatsapp__c param {get;set;}

Valor retornado

Tipo de retorno do get:		ParametroWhatsapp__c.
Tipo do retorno do set:		sem retorno.

response

Get e Set da vari�vel p�blica do tipo String.

Assinatura

public String response {get;set;}

Valor retornado

Tipo de retorno do get:		String.
Tipo do retorno do set:		sem retorno.

WAQrRequest_ctl(std)

Atribui um Par�metro Whatsapp a vari�vel local param.

Assinatura

public WAQrRequest_ctl(ApexPages.StandardController std)

Valor retornado

Sem retorno.

init()

Executa outros m�todos privados da classe.

Assinatura

public void init()

Valor retornado

Sem retorno.
getResponseMessage()

Retorna a mensagem do json feito com o servidor ou Erro inesperado, caso a mensagem esteja vazia.

Assinatura

public String getResponseMessage()

Valor retornado

Tipo:	String.

requestQr() (Acho que essa classe tinha que ser private)

Faz o json de requisi��o de um QR Code para o ParametroWhatsapp__c da vari�vel local param.

Assinatura

public void requestQr()

Valor retornado

Sem retorno.

