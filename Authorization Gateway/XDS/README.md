# How to determine which XSD to Use 

The XSD that will be used can be retrieved from the Terminal Settings, but can also be determined by using the criteria below.   

The root path for all XSDs is http://demo.eftchecks.com/webservices/Schemas followed by the SEC Code and Schema Name. The Schema Name is determined by the following criteria: 

- If the Terminal requires the Driver’s License Information.  
- If the Terminal is configured for Check Verification. 
- If the Terminal is configured for Identity Verification. 

For PPD and CCD entries, If the Terminal is configured to allow Credit entries 

A matrix of the available XSDs for each SEC code can be found in each folder. Each grid contains the name of the schema, based on the schemas determining criteria, and a link to the actual schema.  The grid also includes the Terminal IDs that can be used for testing and certifying against the provided schema. 

An example XSD file path for a PPD terminal that does not require the driver’s license information, is setup for check verification, and is setup for identity verification, and does not allow credits would be as follows:  

https://demo.eftchecks.com/webservices/schemas/ppd/CheckVerificationIdentityVerificationDLOptional.xsd 
