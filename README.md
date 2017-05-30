# Credentials, Cookies, and CORS Quiz.
## Coookieee! Om Nom Nom!

### Instructions
With your partner, in words both of you will understand 6 months from now, answer the following questions.

> How would you best summarize credentials when it comes to auth?

The combination of values associated with a unique identification on a server.

> Describe how cookies are exchanged between client and server.  Make sure you touch on the technical implementation of cookies.

A server will set-cookies in the response header establishing the ability to use cookies. From that point on, the client's browser will send the cookie in the request header to the server keeping the pre-established credentials.

> From the perspective of a developer, name some basic strengths of using cookies and some weaknesses.

Cookies only work with the same-origin (protocol, domain name, port), so sensitive information cannot be accessed by a third-party. Cookies can be intercepted by running JS unless you set then to HTTP-only. Cookies only hold 4KB max (so they're also small enough to transmit quickly).

> What is the difference between a session cookie and a persistant cookie?

Session cookies delete after the browser quits; persistent cookies expire after a set time / event.

> What is your opinion of the same-origin policy?  Support your opinion with some evidence.

Good idea to protect cookie info, and not too arduous to circumvent with CORS exceptions / proxies.

> Based on what you know, how would you explain CORS?

Cross-Origin Resource Sharing is a safe way for vendors to circumvent same-origin policy by creating specific exceptions to AJAX calls & cookie-sharing.
