O WAActionTemplate � o extends obrigat�rio caso queira usar um componente lightning no metadado A��o do Whatsapp do Tipo Messenger. Ele funciona como uma modal, com o layout separado em tr�s partes, cabe�alho, corpo e rodap�.
Nele temos os seguintes atributos:

Entre em Configura��o.
.. image:: WAActionTemplate.png
    :width: 500px
    :alt: Solidity logo
    :align: center

Al�m dos atributos, tem um m�todo para fechamento da modal close().

close()

M�todo utilizado para fechamento da modal.



Exemplo de utiliza��o do componente como extends:

<aura:component extends="whats:WAActionTemplate" >
   <!-- Header -->
   <aura:set attribute="title" value="Relacionar Lead/Contato " />
   <!-- Footer -->
   <aura:set attribute="footer">
       <lightning:button variant="Neutral" label="Cancelar" title="Cancelar" onclick="{! c.close }" />
   </aura:set>

   <!-- Content -->
   <lightning:layout>         
       <!-- LookupField -->
       <lightning:layoutItem flexibility="auto" size="6" >
           <lightning:recordEditForm aura:id="recordViewForm"
               onsubmit="{!c.close}"
               recordId="{!v.conversaWhatsapp.whats__ContatoWhatsapp__c}"
               objectApiName="whats__ContatoWhatsapp__c">
               <lightning:inputField aura:id="lead"
                   fieldName="whats__Lead__c"/>
           </lightning:recordEditForm>
       </lightning:layoutItem>
   </lightning:layout>
</aura:component>

Refer�ncias:
Componente Lightning
WAMessenger
WACoreActionRelacionamento
Metadado
A��o do Whatsapp
Relacionar Contato ou Lead

