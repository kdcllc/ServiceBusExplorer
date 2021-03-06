# Service Bus Explore for Windows Service Bus

Service Bus Explorer code developed by [Paolo Salvatori](https://social.msdn.microsoft.com/profile/paolo%20salvatori/)
The Service Bus Explorer is a tool that you can use to manage and test the entities contained in an Azure Service Bus namespace.

Many Microsoft oriented enterprises still are utilizing the ealier version of what have become known as Azure Service Bus product in the cloud. In its original releases the Service Bus on Windows didn't have any UI tools, 
so [Paolo Salvatori](https://social.msdn.microsoft.com/profile/paolo%20salvatori/) developed the utility to assist the developers' community. Unfortunately, he didn't make the code available in the github, so the
original code base is hard to find. This project space is dedicated to that purpose.

The latest version of this project can be found [here on github.com](https://github.com/paolosalvatori/ServiceBusExplorer)

1. Version 1.8 - is only available as binaries
2. Version 2.0  - https://github.com/kdcllc/ServiceBusExplorer/tree/v2.0.0

###Binaries
1. version 1.8 - https://github.com/kdcllc/ServiceBusExplorer/blob/master/src/1.8.zip 
    (this version provides the ability to pick into message but doesn’t show accurate message count.)
2. version 2.0 - https://github.com/kdcllc/ServiceBusExplorer/blob/master/src/2.0.zip
(This version shows the message counts correctly but can’t peek. 
It pulls the messages which in turns removes them from the queue or a topic.) 
3. version 2.1 - https://github.com/kdcllc/ServiceBusExplorer/blob/master/src/2.1.zip

###Notes
Service Bus doesn’t have any way to see what’s in the queues without a peek and each peek counts against your max received count for message. 
So, if you check what’s on the queue 10 times before a message is actually picked up by a true client, the message gets dead-lettered.

