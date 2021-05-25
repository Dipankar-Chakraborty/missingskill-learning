# Building Block Of Web Components

- [Programming Languages](#Programming-Languages)
- [IP Address](#IP-Address)
- [Port](#Port)
- [Domain](#Domain)
- [Browsers](#Browsers)
- [Code Editor](#Code-Editor)
- [HTTP And HTTPS](#HTTP-And-HTTPS)
- [Web Server](#Web-Server)
- [Web Socket](#Web-Socket)
- [HTTP Verbs](#HTTP-Verbs)
- [HTTP Headers](#HTTP-Headers)
- [HTTP Status Codes](#HTTP-Status-Codes)
- [Software Licenses](#Software-Licenses)
- [Database](#Database)
- [Cloud Providers](#Cloud-Providers)

---
## Programming Languages

Programming languages are used by the developers to develop softwares, scripts or other sets of instructions for computer to execute.

Some of the popular programming languages are:
- **JavaScript** : used for developing both frontend and backend of websites and also to develop android apps
- **SQL** : used for creating and maintaining databases
- **Python** : used for backend development of websites and artificial intelligence development
- **Java** : used for backend development of websites and building android apps
- **Ruby** : used for web application developement
- **C#** : used for automation testing and develop microsoft.net application for windows os 
- **PHP** : used for web application developement
- **Swift** : used for developement of macOS and iOS applications

## IP Address

**An IP (Internet Protocol) address** is a numerical label assigned to the devices connected to a computer network that uses the IP for communication and identifier for a specific machine on a particular network. It also helps to develop a virtual connection between a destination and a source. There are two versions of IP address i.e, IPv4 and IPv6.

**IPv4** was the first version of IP. It was deployed for production in the ARPANET in 1983. The IPv4 uses a **32-bit** address scheme allowing to store 2^32 addresses which is more than 4 billion addresses. Till date, it is considered the primary Internet Protocol and carries most of Internet traffic.

An IPv4 address consists of four numbers, each number contains one to three digits, with a single dot (.) separates each number or set of digits.

IPv4 Address is divided into two parts:

Prefix: The prefix part of IPv4 address identifies the physical network to which the computer is attached. Prefix is also known as a network address.  
Suffix: The suffix part identifies the individual computer on the network. The suffix is also called the host address.  

IPv4 address has **five separate classes** based on four address bits. Here, classes A, B, C offers addresses for networks of three distinct network sizes. Class D is only used for multitasking, and class E reserved exclusively for research and developement purposes.

| Class | Address Range | Subnet Masking | Example IP | Leading Bits  | Max Number Of Networks | Application                            |
| ------| ------------- | -------------  | ---------- | ------------- | ---------------------- | -------------------------------------- |
| A     | 1 to 127      | 255.0.0.0      | 8.8.8.0    | 8             | 128                    | Used for large number of hosts.        |
| B     | 128 to 191    | 255.255.0.0    | 172.1.1.1  | 16            | 16384                  | Used for medium size network.          |
| C     | 192 to 223    | 255.255.255.0  | 192.1.1.1  | 24            | 2097157                | Used for local area network.           |
| D     | 224 to 239    | NA             | 225.1.1.1  | NA            | NA                     | Reserve for multi-tasking.             |
| E     | 240 to 254    | NA             | 245.1.1.1  | NA            | NA                     | Reserved for Research and Development. |

**IPv6** is the recent version of Internet Protocol. This new IP address version is being deployed to fulfill the need for more Internet addresses. It was aimed to resolve issues which are associated with IPv4. With **128-bit** address space, it allows 340 undecillion unique address space. IPv6 also called IPng (Internet Protocol next generation).

## Port

A port is a process-specific or an application-specific software construct serving as a communication endpoint, which is used by User Diagram Protocol (UDP) and Transmission Control Protocol (TCP).A specific network port is identified by its number commonly referred to as port number, the IP address in which the port is associated with and the type of transport protocol used for the communication.

A port number is a 16-bit unsigned integer that ranges from 0 to 65535.
- 0-1023 : reserve ports used by systems
- 1024-49150 : application ports
- 49151-65535 : open ports

Some of the most commonly used ports, along with their associated networking protocol, are:

- **Ports 20 and 21**: File Transfer Protocol (FTP). FTP is for transferring files between a client and a server.
- **Port 22**: Secure Shell (SSH). SSH is one of many tunneling protocols that create secure network connections.
- **Port 25**: Simple Mail Transfer Protocol (SMTP). SMTP is used for email.
- **Port 123**: Network Time Protocol (NTP). NTP allows computer clocks to sync with each other, a process that is essential for encryption.
- **Port 179**: Border Gateway Protocol (BGP). BGP is essential for establishing efficient routes between the large networks that make up the Internet (these large networks are called autonomous systems). Autonomous systems use BGP to broadcast which IP addresses they control.
- **Port 500**: Internet Security Association and Key Management Protocol (ISAKMP), which is part of the process of setting up secure IPsec connections.
- **Port 3389**: Remote Desktop Protocol (RDP). RDP enables users to remotely connect to their desktop computers from another device.

## Domain

**Port 53**: Domain Name System (DNS). DNS is an essential process for the modern Internet; it matches human-readable domain names to machine-readable IP addresses, enabling users to load websites and applications without memorizing a long list of IP addresses.

## Browsers

A browser is a software application used to locate, retrieve, and display content on the World Wide Web, including webpages, images, videos and other files. As a client/server model, the browser is the client run on a computer or mobile device that contacts the Web server and requests information. The web server sends the information back to the browser, which then displays the results on the Internet-enabled device.

Some of the famous browsers are:
- Chrome
- Edge
- Firefox
- Safari
- Brave
- Opera
- Tor

## Code Editor

A Code editor is a text editor program designed to write and edit source code of computer programs by programmers. 

Some of the famous code editors are:
- VS Code
- Sublime Text
- Notepad++
- Codeblocks
- Eclipse
- NetBeans
- Brackets

## HTTP And HTTPS

**Port 80**: Hypertext Transfer Protocol (HTTP). HTTP is the underlying protocol used by the World Wide Web and this protocol defines how messages are formatted and transmitted, and what actions Web servers and browsers should take in response to various commands.
  
**Port 443**: HTTP Secure (HTTPS). HTTPS is the secure and encrypted version of HTTP. All HTTPS web traffic goes to port 443. Network services that use HTTPS for encryption, such as DNS over HTTPS, also connect at this port.

## Web Server

A Web Server is a hardware or software through which a computer can host a website.

Some of the popular web servers are:
- Nginx
- Apache
- Lighttpd

## Web Socket

The WebSocket is an advanced technology that makes it possible to open a two-way interactive communication session between the user's browser and a server. With this, you can send messages to a server and receive event-driven responses without having to poll the server for a reply.
![Web Socket](https://github.com/Dipankar-Chakraborty/missingskill-learning/blob/main/images/web-sockets-visual-representation.jpg)

## HTTP Verbs

HTTP defines a set of request methods to indicate the desired action to be performed for a given resource, referred as HTTP Verbs.
- **GET** : GET method requests a representation of the specified resource. Requests using GET should only retrieve data.
- **HEAD** : HEAD method asks for a response identical to that of a GET request, but without the response body.
- **POST** : POST method is used to submit an entity to the specified resource, often causing a change in state or side effects on the server.
- **PUT** : PUT method replaces all current representations of the target resource with the request payload.
- **DELETE** : DELETE method deletes the specified resource.
- **OPTIONS** : OPTIONS method is used to describe the communication options for the target resource.

## HTTP Headers

HTTP headers let the client and server pass additional information with an HTTP request or response.

## HTTP Status Codes

HTTP Status Codes indicate whether a specific HTTP request has been successfully completed.

Status codes are grouped in five classes
- Informational responses
  - 100 - Continue
- Successfull responses
  - 200 - OK
  - 201 - Created
  - 202 - Accepted
- Redirects
  - 301 - Moved Permanently
  - 302 - Found
- Client errors
  - 400 - Bad Request
  - 401 - Unauthorized
  - 403 - Forbidden
  - 404 - Not Found
- Server errors
  - 500 - Internal Server Error
  - 502 - Bad Gateway
  - 503 - Service Unavailable
  - 504 - Gateway Timeout

## Software Licenses

A Software license is legal instrument governing the use and redistribution of software.

Some of the open source, free licenses are:
- Apache
- MIT
- BSD
- GPL
- Mozilla

## Database

Database is a tool for collecting and organizing information. Databases can store information about people, products, orders or anything else.

There are two types of databases relational and non-relational.  
**Relational Databases:**
- MySql
- PostgreSQL
- MariaDB  

**Non-Relational Databases:**
- MongoDB
- Redis
- Cassandra
- NeoJS

## Cloud Providers

A cloud service provider is a third-party company offering a cloud-based platform, infrastructure, application, or storage services. Ccompanies typically have to pay only for the amount of cloud services they use, as business demands require.

Some of the popular cloud service providers are:
- AWS
- Google Cloud
- Azure
- BlueMix
- DigitalOcean
- Vultr
- Linode
- Heruko

---
