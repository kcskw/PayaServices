# 12.0 How to determine which XML Template to Use 

The XML data packet can be built from scratch by the web service consumer or one of the available XML templates can be used to build the XML data packet prior to submitting the data packet to the Authorization Gateway. The URI for the XML data packet for a given terminal can be retrieved from the Terminal Settings but can also be determined by using the criteria below. 

The root path for all XML Templates is https://demo.eftchecks.com/webserivces/schemas/  followed by the SEC Code, “/Templates/”, and the XML Template name.  The XML Template is determined by the following criteria: 

- If the Terminal requires the Driver’s License Information. 
- If the Terminal is configured for Check Verification. 
- If the Terminal is configured for Identity Verification. 

A matrix of the available XML Templates for each SEC code can be found below. Each grid contains the name of the XML Template, based on the XML Templates determining criteria, and a link to the actual XML Template.  

The grid also includes the Terminal IDs that can be used for testing and certifying the XML data packet that can be built from the provided XML Template. The Terminal ID will be different for guaranteed transactions and Non-guaranteed transactions.  Guaranteed terminals are numbered 1xxx, and Non-guaranteed terminals are numbered 2xxx. 
