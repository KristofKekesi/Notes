HTTP response status codes are the indicators of whether an action has been successfully completed or not.
## 100 (Informational responses)
- #### 100: Continue
	Indicates that the client should continue the HTTP request or ignore the response if the request is already finished.
- #### 101: Switching Protocols
	==Only available in Upgrade header in HTTP/1.1==
	This code is sent by the client and indicates the protocol that it's switching to.
- #### 102: Processing
	==Only available in the HTMP extension WebDAV (Web Distributed Authoring and Versioning)==
	This code indicates that the server has received and is processing the request, but no response is available yet.
- #### 103: Early Hints ==(Experimental)==
	This code is primarily intended to be used with the Link header, letting the user-agent start preloading resources while the server prepares a response.
## 200 (Successful responses)
- #### 200: OK
	The request succeeded. The meaning of success depends on the HTTP method.
	- [[HTTP request types#GET|GET]]: The resource has been fetched and transmitted in the message body.
	- HEAD: The representation headers are included in the response without any message body.
	- [[HTTP request types#PUT|PUT]] or [[HTTP request types#POST|POST]]: The resource describing the result of the action is transmitted in the message body.
	- TRACE: The message body contains the request message as received by the server.
## 300 (Redirection messages)
## 400 (Client error responses)
## 500 (Server error responses)