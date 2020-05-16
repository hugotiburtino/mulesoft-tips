# MuleSoft Tips

Some lessons from the experience with MuleSoft

## Salesforce Connector
* I would in principle avoid the 'On new object' component. 
The default time may cause your Salesforce account to get locked, since it would ping Salesforce every minute. 
If you have to use it, extend the time of ping.


