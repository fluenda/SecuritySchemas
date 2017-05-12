# Security Schemas
A hub for AVRO compatible schemas for different vendor log formats

Published schemas:
* [CEFRev23](CEFRev23) 

  AVRO Schema representation of the Common Event Format as specified by the following document:
  
  https://www.protect724.hpe.com/servlet/JiveServlet/downloadBody/1072-102-9-20354/CommonEventFormatv23.pdf

  The Simplified schema is flat (i.e. Header and Extensions are part of the same POJO) and all CEF complex types 
   (i.e. MacAddress, DateTime, etc) are converted to Strings. 
   
   Also note the schema performs no validation being essential that software making use of the schema perform
    validation prior to writting into and/or after reading data utilising this schema. 