WAQrView_ctl

param

Get e Set da vari�vel p�blica do tipo ParametroWahtsapp__c.

Assinatura

public ParametroWhatsapp__c param {get;set;}

Valor retornado

Tipo de retorno do get:		ParametroWhatsapp__c.
Tipo do retorno do set:		sem retorno.

keepPolling

Get e Set da vari�vel p�blica do tipo Boolean.

Assinatura

public Boolean keepPolling {get;set;}

Valor retornado

Tipo de retorno do get:		Boolean.
Tipo do retorno do set:		sem retorno.

WAQrView_ctl(std)

Atribui um Par�metro Whatsapp a vari�vel local param.

Assinatura

public WAQrView_ctl(ApexPages.StandardController std)

Valor retornado

Sem retorno.

init()

Executa outros m�todos privados da classe.

Assinatura

public void init()

Valor retornado

Sem retorno.

loadQr()

Carrega a imagem do QR Code do Par�metro Whatsapp da vari�vel local param.

Assinatura

public void loadQr()

Valor retornado

Sem retorno.

getCurrentQrId()

Retorna o Id da imagem do QR Code do Par�metro Whatsapp da vari�vel local param.

Assinatura

public Id getCurrentQrId()

Valor retornado

Tipo: 	Id.

getDisplayMessage()

Retorna a mensagem �Aguardando QR Code...� caso esteja aguardando o QR Code e retorna a mensagem �Nenhum c�digo dispon�vel� caso a organiza��o n�o esteja ativada no servidor ou se o Par�metro Whatsapp j� esteja conectado.

Assinatura

public String getDisplayMessage()

Valor retornado

Tipo: 	String.

