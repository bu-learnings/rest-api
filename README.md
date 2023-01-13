# rest-api

## Intro
* REST API - **RE**presentational **S**tate **T**ransfer,it is a way to communicate between computer and server 
___
## Different types of REST API
| Type  | Function  |
|----   |---          |
| POST | **C**reate         |
|  GET  | **R**ead      |
| PUT | **U**pdate     |
|DELETE | **D**elete|
___
## HTTP response status codes
>### Informational responses (100 – 199)
>#### 100 Continue
>* indicates that the client should continue the request or ignore the response if >the request is already finished.
>#### 101 Switching Protocols
>* This code is sent in response to an Upgrade request  from the client and indicates the protocol the server is switching to.

>### Successful responses (200 – 299)
>#### 200 OK
>* The request succeeded
>#### 201 Created
>* The request succeeded, and a new resource was created as a result
>#### 202 Accepted
>* The request has been received but not yet acted upon
>#### 203 Non-Authoritative Information
>* This response code means the returned metadata is not exactly the same as is available from the origin server, but is collected from a local or a third-party copy.
>#### 204 No Content
>* There is no content to send for this request
>#### 205 Reset Content
>* Tells the user agent to reset the document which sent this request.
>#### 206 Partial Content
>* This response code is used when the Range header is sent from the client to request only part of a resource.

>### Redirection messages (300 – 399)

>### Client error responses (400 – 499)
>#### 400 Bad Request
>* The server cannot process the request due to client error
>#### 401 Unauthorized
>* The client must authenticate itself to get the requested response.
>#### 402 Payment Required Experimental
>* This response code is reserved for future use. The initial aim for creating this code was using it for digital payment systems, however this status code is used very rarely and no standard convention exists.
>#### 403 Forbidden
>* The client does not have access rights to the content; that is, it is unauthorized, so the server is refusing to give the requested resource. Unlike 401 Unauthorized, the client's identity is known to the server.
>#### 404 Not Found
>* The server cannot find the requested resource. In the browser, this means the URL is not recognized. In an API, this can also mean that the endpoint is valid but the resource itself does not exist. 
>#### 405 Method Not Allowed
>* The request method is known by the server but is not supported by the target resource. For example, an API may not allow calling DELETE to remove a resource.
>#### 407 Proxy Authentication Required
>* This is similar to 401 Unauthorized but authentication is needed to be done by a proxy.
>#### 408 Request Timeout
>* This response is sent on an idle connection by some servers, even without any previous request by the client. It means that the server would like to shut down this unused connection.
>#### 409 Conflict
>* This response is sent when a request conflicts with the current state of the server.

>### Server error responses (500 – 599)
>#### 501 Not Implemented
>* The request method is not supported by the server and cannot be handled.
>#### 502 Bad Gateway
>* This error response means that the server, while working as a gateway to get a response needed to handle the request, got an invalid response.
>#### 503 Service Unavailable
>* The server is not ready to handle the request. Common causes are a server that is down for maintenance or that is overloaded.
>#### 504 Gateway Timeout
>* This error response is given when the server is acting as a gateway and cannot get a response in time.
>#### 505 HTTP Version Not Supported
>* The HTTP version used in the request is not supported by the server.
___
## Token generation for POSTMAN
* Click Profile -> Settings -> Dev settings-> Personal access token
* Click on tokens and generate new tokens
* Fill in the name and check on repo -> click generate token
* Copy the token and open POSTMAN App
* Click **New** -> **HTTP Request** -> Select POST -> enter url (https://api.github.com/repos/OWNER/REPO/branches)  where OWNER=Organization, REPO=GitHub Repo
* Select **Authorization** -> Select **Type** as **Bearer Token** -> Paste copied token
* Select **Body** -> click **raw** -> select JSON -> enter the body 
___
## Token : 
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 \
(after uploading the token, github revoked the token and requested to generate a new token)
___
