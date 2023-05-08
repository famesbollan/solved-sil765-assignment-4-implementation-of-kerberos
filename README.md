Download Link: https://assignmentchef.com/product/solved-sil765-assignment-4-implementation-of-kerberos
<br>
You are required to (a) build an AS, a TGS, an application server (indeed a web server), and (b) build one or more clients that wish to connect to the application server using the services of the AS and TGS (Please see slides on Kerberos)

To do so, you will need to:

<ul>

 <li>ensure that AS and TGS have the required information concerning the server(s) and the clients,</li>

 <li>AS, TGS, the servers and clients are able to generate/interpret tickets and thus provide services to clients as when sought.</li>

</ul>

Note, access to the server (in this case a web server) requires authentication.

Once a session key has been established between a client and the web application server, the client can download the home page of the web server.

Project no. 2: Diffie‐Hellman key generation and exchange

You are required to build clients A and B that wish to send messages from B to A (only B to A) but encrypted using Elgamal Cryptosystem, but only after having exchanged messages that finally result in computation of <u>one‐time</u> keys using the Diffie Hellman protocol. (Pl. refer to relevant slides from Lecture 8 Part 1.)

The Elgamal Cryptosystem uses the parameters (q, a). These are known to each other using “other means”.

To ensure that man‐in‐the‐middle attack is not possible, the two clients A and B send <u>initial</u> messages to each other by adding to each message a MAC (or an “integrity check”) that itself is based on HMAC algorithm and uses a shared

“secret”.

To do so, you will need to:

<ul>

 <li>ensure that clients already (somehow) know the shared “secret” to be used with HMAC,</li>

 <li>assume that Diffie‐Hellman parameters (q, a) are already fixed, and known to them,</li>

 <li>(once they know how to generate or compute one‐time passwords) messages sent from B to A are encrypted using Elgamal cryptosystem with parameters, (q, a).</li>

</ul>

Once the one‐time keys have been computed (or can be computed on the fly), B should encrypt and send messages

“hello 1”, “hello 2”, “hello 3”.


