# MuleSoft Tips

Some lessons from the experience with MuleSoft

## Finding Help
[MuleSoft Help Center](https://help.mulesoft.com/s/) has obviously much more entries than Stackoverflow. 

## Salesforce Connector
* Avoid the 'On new object' component. 
The default time may cause your Salesforce account to get locked, since it would ping Salesforce every minute. 
If you have to use it, extend the time of ping.
* If you need to synchronize Salesforce with something else (let's say SAP), subscription (like 'Replay Topic' or 'Subscribe channel') is a much better way to do that than 'On New Object'.

## SAP Connector
* The SAP service __API_BusinessPartner__ has to be activated by the SAP team. After that, the connection to MuleSoft takes place smoothly. If you have/want to use other service, ask the SAP team to configure it properly, preferably like the API_BusinessPartner.
