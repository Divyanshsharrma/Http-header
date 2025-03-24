# Http-header

List the http headers, their purpose and what will be the result of its absence.
Working of HTTP is based on Request-Response behavior, There are two types of Http Header format: 

1.Request Header : Sent from Client to the Web server contains information about the client's request, such as cookies and the browser being used etc 
2. Response Header : Sent form web server to the client contains information about the server's response, such as content type, caching, instructions and status codes etc.

List of HTTP headers, their purposes and their absence results : 
. Host : 
purpose  - Indicates which server the client wants to communicate with. 
Absence  - Sever unable to determine which domain is being requested which leads to bad request error. 

.Content-Type :
purpose - Ensures the server understands how to process the data being sent by the client Absence Impact - server may not understand the data format, leading to processing erros 

.Cookie : 
purpose - sends stored http cookies from the client to the server, maintains session rate and user preferences between requests.
absence impact - may not recognize the client's session, leading to the need to reauthenticate. 

.Cache Control : 
purpose - specifies caching policies such as expiration times and revalidation requirements. absence impact - cache store responses inapporiately leads to unoptimized content delivery. 

.Server : 
purpose - identifies the web server software and sometimes includes the version number. 
absence impact - potential attackers cannot easily identify the server type, reducing their ability to exploit server-specific vulnerabilities. 

.path :
purpose - Web servers and APIs use the path to route requests to the appropriate handler or service. 
absence impact - 404 Not Found Error: If no path is provided, the server cannot identify the requested resource. 

.priority :
purpose - Determines how urgent the resource is. Lower values indicate higher urgency absence impact - the server decides resource delivery order, which may slow down page load times. 

.Accept-Encoding :
purpose - Tells the server which compression algorithms the client can understand.
absence impact - The server will send uncompressed data, increasing load times and bandwidth usage 

.Accept-language :

purpose - Enables the server to provide content in the user's preferred language. 
absence impact -  Users may receive content in a non-preferred language.

#Screenshot of http header section in Buirpsuite
![http header](https://github.com/user-attachments/assets/d4bb9ecc-045c-4f11-ad5e-0d0a3369edfa)



