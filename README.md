#  Sip Signalling Part 1 

# Client-Server Model 

- [SIP Clients and Server]()

# SIP Requests 

- [SIP Request Message]()
  * [Methods]()
  * * [INVITE]()
  * * [REGISTER ]()
  * * [CANCEL]()
  * * [BYE ]()
  * * [ACK ]()
  * * [OPTIONS ]()
  * * [REFER]()
  * * [SUBSCRIBE]()
  * * [NOTIFY]()
  * * [MESSAGE ]()
  * * [INFO]()
  * * [PRACK]()
  * * [UPDATE]()
  

# SIP Responses 

 [SIP Response Message]()
 * [Informational]()
 * * []()
 * * []()
 * * []()
 * * []()
 * * []()
 * [Success]()
 * * []()
 * * []()
* [Redirection]()
 * * []()
 * * []()
 * [Client Error]()
 * * []()
 * * []()
 * * []()
* [Server Error]()
* * []()
* * []()
* * []()
* [Global Error]()
* * []()
* * []()
* * []()

# SIP Header Fields

- [SIP Header Fields]()

# Basic Call Flows


# Introduction to everthing
This part of the project covers SIP Understanding the Session Initiation Protocol book (author Alan B. Johnston) as well as the RFC 3261.

Best Materials about the SIP and VOIP network;

* SIP Understanding the Session Initiation Protocol book (author Alan B. Johnston)
* RFC 3261 
* [Eli the Computer Guy VOIP series](https://www.youtube.com/watch?v=2x3Ie6VZ_sg&list=PLUz96g7K7QmkOOnUkzUkvT8RcFpP08oE0)

# What is SIP

<pre>
The Session Initiation Protocol (SIP) is a signaling, presence and instant messaging protocol developed to set up, modify, and tear down multimedia sessions, request and deliver presence and instant messages over the Internet.


SIP was developed by the IETF as part of the Internet Multimedia Conferencing Architecture, and was designed to dovetail with other Internet protocols such as Transmission Control Protocol (TCP), Transmission Layer Security (TLS), User Datagram Protocol (UDP), Internet Protocol (IP), Domain Name System (DNS), and others. 


As the name implies,the protocol allows two end points to establish media sessions with each other. 

The main signaling functions of the protocol are as follows: 

• Location of an end point;
• Contacting an end point to determine willingness to establish a session; 
• Exchange of media information to allow session to be established; 
• Modification of existing media sessions;
• Tear-down of existing media sessions.

SIP is a client-server protocol of equipotent peers.
</pre>
# What is Client-Server architecture

- [x] What is Client-Server
- [ ] Add images
- [ ] Open a pull request
<pre>
The client component requests services from the server.

The server component provides a function or service to one or many clients, which initiate requests for such services. Servers are classified by the services they provide.

Clients and servers exchange messages in a request–response messaging pattern. The client sends a request, and the server returns a response.This exchange of messages is an example of inter-process communication. To communicate, the computers must have a common language, and they must follow rules so that both the client and the server know what to expect. The language and rules of communication are defined in a communications protocol. In this case, our communication protocol is SIP.

</pre>

# What is User Agent / User Agent Client (UAC) / User Agent Server (UAS)
<pre>
User Agent : A user agent represents an end system. It can be either user agent client or user agent server.
User Agent Client (UAC) : Generates requests.
User Agent Server (UAS) : Responds to the requests.  
</pre>
# Requests

- [x] Requests
- [ ] Methods
- [ ] Add Methods
- [ ] Create images
- [ ] Add images

<pre>
This chapter is created by using the RFC 3261. 

Request is a SIP message sent from a client to a server, for the purpose of invoking a particular operation.

SIP requests are distinguished by having a Request-Line for a start-line.

         Request-Line  =  Method SP Request-URI SP SIP-Version CRLF

A Request-Line contains a method name, a Request-URI, and the  protocol version separated by a single space (SP) character.

Example of a Request-Line:

INVITE sip:watson@bell-telephone.com SIP/2.0

In this below example;

INVITE : Method name
sip:watson@bell-telephone.com : Request-URI
SIP/2.0 : SIP-Version
</pre>
## Methods 
<pre>
This specification defines six methods:
 REGISTER for registering contact information, INVITE, ACK, and CANCEL for setting up sessions, BYE for terminating sessions, and OPTIONS for querying servers about their capabilities. 
</pre>

## INVITE
The INVITE method is used to establish media sessions between user agents.


