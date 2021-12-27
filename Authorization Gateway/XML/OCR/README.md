## 12.4 OCR XML Templates 

There are two different ways of processing images, one with OCR and one with Mobile OCR.  Images captured by a Mobile Device are handled differently (due to patent restrictions) than images captured via a desktop scanner, such as an RDM, Panini, Magtek or other peripheral device.  Images submitted via a mobile device must be submitted as a .JPG, while images submitted via a peripheral device must be submitted in a .TIFF format.   

Images submitted via a Mobile device, will have the MICR, Courtesy Amount, and Legal Amount recognized by the standard Mobile OCR function.  In order to submit for FULL OCR to receive the additional fields (Payee, Address, Endorsement, etc.), it will be necessary that you code for the full set of OCR responses.     

A matrix of the available XML Templates when using OCR for each SEC code can be found in each folder. Each grid contains the name of the XML Template, based on the XML Templates determining criteria, and a link to the actual XML Template. The Trans Type will indicate what type of response you should receive. NOTE: Verify Check can be applied to any terminal. This will NOT impact the terminal schemas or template. 

Trans Type: 
- P – Successful Transaction 
- O -  Successful Transaction with failed optional fields (Fields that are not required to pass the transaction in the system. NOTE: Fields may not match image depending on how OCR translates the image). 
- F – Failed Transaction 
- **Note:  Optional values submitted for OCR will be TRUSTED and not validated by OCR**
