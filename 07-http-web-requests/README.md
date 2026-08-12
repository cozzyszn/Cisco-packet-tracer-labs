# Packet Tracer - Observe Web Request

## Objective

Observe the client/server traffic generated when a PC requests web services from a web server using Cisco Packet Tracer.

## Lab Overview

In this exercise, I investigated how a client communicates with a web server to access a webpage. I used DNS, ICMP, TCP, and HTTP traffic to understand the different stages involved in a web request.

## Tasks Completed

### 1. Verify Connectivity

- Used the `ping` command from the External Client.
- Pinged `ciscolearn.web.com`.
- Observed that the domain name was resolved to an IP address through DNS.
- Verified connectivity between the client and the web server.

### 2. Connect to the Web Server

- Opened the Web Browser on the External Client.
- Accessed `ciscolearn.web.com`.
- Observed the webpage returned by the web server.

### 3. View HTML Code

- Opened the web server.
- Navigated to `Services > HTTP`.
- Viewed the `index.html` file.
- Compared the HTML code with the webpage displayed in the browser.

### 4. Observe Network Traffic

- Switched Cisco Packet Tracer to Simulation Mode.
- Filtered the traffic to display TCP and HTTP.
- Created a Complex PDU from the External Client to the web server.
- Configured HTTP as the application.
- Set the starting source port to `1000`.
- Used a periodic interval of `120 seconds`.
- Played the simulation and observed the packets travelling between the client and server.

## Networking Concepts

| Concept | What I Learned |
|---|---|
| DNS | Resolves a domain name to an IP address |
| IP Addressing | Identifies the source and destination devices |
| ICMP | Used by ping to test connectivity |
| TCP | Provides reliable communication between client and server |
| HTTP | Used to request and deliver web content |
| HTML | Defines the structure of the webpage |
| Client/Server | The client requests resources and the server provides them |
| PDU | Represents data exchanged between network devices |

## Observations

The web request generated multiple packets because HTTP operates over TCP. TCP requires connection establishment and acknowledgements to provide reliable communication.

The simulation showed that communication between the client and web server involves more than simply sending a request. Multiple packets are exchanged during the communication process.

## Key Takeaways

This lab helped me understand the relationship between DNS, IP addressing, TCP, and HTTP during a web request.

The general communication process can be summarized as:

**Client → DNS Resolution → Server IP Address → TCP Connection → HTTP Request → HTTP Response → Webpage**

## Files

- `observe-web-request.pkt` - Cisco Packet Tracer lab file
- `screenshots/` - Screenshots showing the different stages of the exercise
