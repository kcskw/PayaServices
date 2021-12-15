# **Overview**

The Application Gateway is designed to accommodate various input requirements. This allows for the development of a single interface that can be easily configured to handle many different scenarios.

The Application Gateway uses web services to present distributed methods for integration into client applications, and an interface with the Application Gateway can be developed with any programming language that can consume a web service.

Extensible Markup Language (XML) is used to send data packet requests to the Authorization Gateway and to receive a response back.  Simple Object Access Protocol (SOAP) is used for XML message exchange over HTTPS. The Application Gateway also employs a custom SOAP header for authentication information. 

# **Connection Method**
Paya Services supports connection via secure (https) webservice using SOAP.  SOAP is a simple XML-based protocol to let applications exchange information over HTTP.  
The webservice address used for certification and testing is as follows:

https://demo.eftchecks.com/webservices/AppGateway.asmx

A username and password for certification will be provided upon request.

_NOTE:  A live webservice address, username, and password will be supplied upon successful certification._

# **Supported Electronic Applications**
 - Telephone Initiated Entry (TEL)
 - Internet Initiated Entry (WEB)
 - Prearranged Payment and Deposit Entry (PPD)
 - Corporate Credit or Debit (CCD)
 - Point-of-Purchase Entry (POP)
 - Check 21 (C21) 
 - Gift Card

# **Submission**
The Application Gateway has been designed for fast and easy integration with your existing system.  Simply create an xml data packet that conforms to the NewMerchApp xsd and pass it to the Application Gateway for processing. To accomplish this the Application Gateway provides 2 web methods: one for certification and one for production.  In addition, each web method contains a custom SOAP header used for authentication.

## **SOAP Header**

|                 |               |                                                                |
|-----------------|---------------|----------------------------------------------------------------|
|     UserName    |     String    |     Username   provided by Paya Services for authorization.    |
|     Password    |     String    |     Password   provided by Paya Services for authorization.    |

(Please Holder Example) 

# **Web Methods**

A definition of the web methods can be found below. Each web method contains a hyperlink to a sample SOAP request and response.

_NOTE: Board Location and Board Terminal will use the Data from Board Merchant._

## **ACH Certification Methods**

- [**BoardCertificationMerchant_ACH**](https://demo.eftchecks.com/webservices/AppGateway.asmx?op=BoardCertificationMerchant_ACH)

  - **Description**:  This method will process an ACH merchant application and return a detail success or failure response.  This method is used during interface testing and certification.  
  - **Input**: Accepts an XML string called a data packet that much conform to the application schema.  
  - **Output**:  Outputs an XML string.

- [**BoardCertificationLocation_ACH**](https://demo.eftchecks.com/webservices/AppGateway.asmx?op=BoardCertificationLocation_ACH)
  - **Description**:  This method will process an ACH location application and return a detail success or failure response.  This method is used during interface testing and certification.  
  - **Input**:  
    - Paya Services Merchant ID as Integer
    - Accepts an XML string called a data packet that must conform to the new terminal application schema.
  - **Output**:  Outputs an XML string.

- [**BoardCertificationTerminal_ACH**](https://demo.eftchecks.com/webservices/AppGateway.asmx?op=BoardCertificationTerminal_ACH)
  - **Description**:  This method will process an ACH terminal application to add a terminal to an EXISTING merchant location and return a detail success or failure response.  This method is used during interface testing and certification.
  - **Input**:  
    - Paya Services Location ID as Integer
    - Accepts an XML string called a data packet that must conform to the new terminal application schema.
  - **Output**:  Outputs an XML string.

- [**CreateCertificationTerminal_ACH**](https://demo.eftchecks.com/webservices/AppGateway.asmx?op=CreateCertificationTerminal_ACH)
  - **Description**:  This method will process an ACH terminal application to add a terminal to an EXISTING merchant location and return a detail success or failure response. It does not require a terminal to clone. The method also allows a terminal to be boarded for a new Program. This method is used during interface testing and certification.
  - **Input**:  
    - Paya Services Location ID as Integer
    - Accepts an XML string called a data packet that must conform to the new terminal application schema.
  - **Output**:  Outputs an XML string.

## **Check21 Certification Methods**

- [**BoardCertificationMerchant_Check21**](https://demo.eftchecks.com/webservices/AppGateway.asmx?op=BoardCertificationMerchant_Check21)
  - **Description**:  This method will process a Check21 merchant application and return a detail success or failure response.  This method is used during interface testing and certification.  
  - **Input**:  Accepts an XML string called a data packet that much conform to the application schema.  
  - **Output**:  Outputs an XML string.

- [**BoardCertificationLocation_Check21**](https://demo.eftchecks.com/webservices/AppGateway.asmx?op=BoardCertificationLocation_Check21)

  - **Description**:  This method will process a Check21 location application and return a detail success or failure response.  This method is used during interface testing and certification.  
  - **Input**:  
    - Paya Services Merchant ID as Integer
    - Accepts an XML string called a data packet that must conform to the new terminal application schema.
  - **Output**:  Outputs an XML string.

- [**BoardCertificationTerminal_Check21**](https://demo.eftchecks.com/webservices/AppGateway.asmx?op=BoardCertificationTerminal_Check21)

  - **Description**:  This method will process a Check21 terminal application to add a terminal to an EXISTING merchant location and return a detail success or failure response.  This method is used during interface testing and certification.
  - **Input**:  
    - Paya Services Location ID as Integer
    - Accepts an XML string called a data packet that must conform to the new terminal application schema.
  - **Output**:  Outputs an XML string.

- [**CreateCertificationTerminal_Check21**](https://demo.eftchecks.com/webservices/AppGateway.asmx?op=CreateCertificationTerminal_Check21)

  - **Description**:  This method will process a Check21 terminal application to add a terminal to an EXISTING merchant location and return a detail success or failure response. It does not require a terminal to clone. The method also allows a terminal to be boarded for a new Program. This method is used during interface testing and certification.
  - **Input**:  
    - Paya Services Location ID as Integer
    - Accepts an XML string called a data packet that must conform to the new terminal application schema.
  - **Output**:  Outputs an XML string.

## **Gift Certification Methods**

- [**BoardCertificationMerchant_Gift**]()
- 
  - **Description**:  This method will process a Gift merchant application and return a detail success or failure response.  This method is used during interface testing and certification.  
  - **Input**:  Accepts an XML string called a data packet that much conform to the application schema.  
  - **Output**:  Outputs an XML string.

- [**BoardCertificationLocation_Gift**]()
  - **Description**:  This method will process a Gift location application and return a detail success or failure response.  This method is used during interface testing and certification.  
  - **Input**:  
    - Paya Services Merchant ID as Integer
    - Accepts an XML string called a data packet that must conform to the new terminal application schema.
  - **Output**:  Outputs an XML string.

- [**BoardCertificationTerminal_Gift**]()
  - **Description**:  This method will process a Gift terminal application to add a terminal to an EXISTING merchant location and return a detail success or failure response.  This method is used during interface testing and certification.
  - **Input**:  
    - Paya Services Location ID as Integer
    - Accepts an XML string called a data packet that must conform to the new terminal application schema.
  - **Output**:  Outputs an XML string.

- [**CreateCertificationTerminal_Gift**]()
  - **Description**:  This method will process a Gift terminal application to add a terminal to an EXISTING merchant location and return a detail success or failure response. It does not require a terminal to clone. The method also allows a terminal to be boarded for a new Program.  This method is used during interface testing and certification.
  - **Input**:  
    - Paya Services Location ID as Integer
    - Accepts an XML string called a data packet that must conform to the new terminal application schema.
  - **Output**:  Outputs an XML string.
