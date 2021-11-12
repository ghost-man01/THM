# Whois

Domain name -- the unsung saviors of Internet.

Whois essentially allows you to query who a domain name is registered to 
Web version of [whois](https://whois.com/whois)

# Dig
How an URL get converted into an IP address that your computer can understand?
The answer is TCP/IP protocol called DNS(Domain Name System)

## DNS
DNS allows us to ask a special server to give us the IP address of the website we're trying to access. 

Example -> If we made a request to www.google.com our server would first send a request to a special DNS server(which your computer knows how to find). The server would then go looking for the IP address for Google and send it back to us. Our computer could then send the request to the IP of the Google Server.  

When you requested a website in your computer firstly it check for **local cache** to see if it's already got an IP address stored for the website. 

Assuming address not previously found, your computer will then send a request to what's knows as recursive DNS server. If the website you've request isn't stored in cache the recursive server will pass the request on to a **root name server.**
The root name server essentially keep track of your DNS servers in the next level down, choosing an appropriate one to redirect your request to. The lower level server are called **Top level Domains(TLDs)**.
TLD server keep track of the next level down : **Authoritative** name servers 
When TLD server receives your request for information the server will passes it down to an appropriate *Authoritative name server*
This all happens automatically when you visit a website but we do it manually with a #Tools *dig*.

Dig allow us manually query recursive DNS servers of our choice for information about domain :
Usage : 	dig \<domain> @\<dns-server-ip>
This is very powerful tool for network troubleshooting.

![[Pasted image 20211112123910.png]]

Interesting piece of information that *dig* give us **Time To Live (TTL)** of the queried dns record. TTL is measured in *seconds*

