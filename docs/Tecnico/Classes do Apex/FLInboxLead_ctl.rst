#################
FLInboxLead_ctl
#################

doExecuteAction()
---------------

Assinatura
    @AuraEnabled
    public static void doExecuteAction(AcaoFalae__mdt pAcaoFalae, ConversaFalae__c pConversaFalae)
Ação
    Executa a ação determinado no pelo metadado AcaoFalae__mdt enviado por parâmetro
Exemplo

   .. code-block:: apex
   
       List<ConversaFalae__c> lstChanged = new List<ConversaFalae__c>([
                                                                        SELECT 
                                                                                Id, 
                                                                                Name, 
                                                                                ContatoFalae__r.Name,                   
                                                                                ContatoFalae__r.Numero__c, 
                                                                                ParametroFalae__r.NumeroCompleto__c, 
                                                                                ParametroFalae__r.Name, 
                                                                                Status__c 
                                                                        FROM 
                                                                                ConversaFalae__c
                                                                        ]);
      AcaoFalae__mdt pAcaoFalae = new AcaoFalae__mdt();
      FLInboxLead_ctl.doExecuteAction(pAcaoFalae, lstChanged[0]);
      
getCurrentUser()
---------------

Assinatura
    @AuraEnabled
    public static User getCurrentUser()
Ação
    Retorna o Usuário conectado.
Retorno
    Retorna um objeto do tipo User
Exemplo

   .. code-block:: apex

      FLInboxLead_ctl.getCurrentUser();
      
getFLActions()
---------------

Assinatura
    @AuraEnabled
    public static List<AcaoInbox> getFLActions(ConversaFalae__c pConversaFalae)
Retorno
    Retorna uma lista com as informações de AcaoFalae__mdt do tipo Inbox
Retorno
    Retorna o Usuário List<**AcaoInbox**>.    
Exemplo

   .. code-block:: apex

      List<ConversaWhatsapp__c> lstChanged = new List<ConversaWhatsapp__c>([
                                                                            SELECT 
                                                                                    Id, 
                                                                                    Name, 
                                                                                    AgenteResponsavel__c, 
                                                                                    ContatoWhatsapp__r.Name, 
                                                                                    ContatoWhatsapp__r.Numero__c, 
                                                                                    ParametroWhatsapp__r.Celular__c, 
                                                                                    ParametroWhatsapp__r.Name, 
                                                                                    Status__c 
                                                                            FROM 
                                                                                    ConversaWhatsapp__c
                                                                          ]);
      FLInboxLead_ctl.getWAActions(lstChanged[0]);
