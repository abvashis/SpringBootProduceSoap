
https://howtodoinjava.com/spring/spring-boot/spring-boot-soap-webservice-example/

http://www.springboottutorial.com/creating-soap-web-service-with-spring-boot-web-services-starter


wsdl : http://localhost:8080/service/studentDetailsWsdl.wsdl

Request :
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:sch="https://www.howtodoinjava.com/xml/school">
   <soapenv:Header/>
   <soapenv:Body>
      <sch:StudentDetailsRequest>
         <sch:name>Sajal</sch:name>
      </sch:StudentDetailsRequest>
   </soapenv:Body>
</soapenv:Envelope>

URL:
http://localhost:8080/service/student-details

POST

Response:
<SOAP-ENV:Envelope xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/">
   <SOAP-ENV:Header/>
   <SOAP-ENV:Body>
      <ns2:StudentDetailsResponse xmlns:ns2="https://www.howtodoinjava.com/xml/school">
         <ns2:Student>
            <ns2:name>Sajal</ns2:name>
            <ns2:standard>5</ns2:standard>
            <ns2:address>Pune</ns2:address>
         </ns2:Student>
      </ns2:StudentDetailsResponse>
   </SOAP-ENV:Body>
</SOAP-ENV:Envelope>