# Class 33

**JSON Web Tokens**

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

**DRF JWT Authentication**

The JWT is acquired by exchanging an username + password for an access token and an refresh token. The access token is usually short-lived (expires in 5 min or so, can be customized though). The refresh token lives a little bit longer (expires in 24 hours, also customizable). It is comparable to an authentication session. After it expires, you need a full login with username + password again. It’s a security feature and also it’s because the JWT holds a little bit more information.

**Django Runserver Is Not Your Production Server**

The server started with runserver is not guaranteed to be performant (it’s very slow), and it hasn’t been built with security concerns in mind. Not a good fit for production use.

A production setup usually consists of multiple components, each designed and built to be really good at one specific thing. They are fast, reliable and very focused. When a request arrives at your server, it should be passed to a dedicated web server. Nginx is an example for a good web server. If you want to run Django in production, be sure to use a production-ready web server like Nginx, and let your app be handled by a WSGI application server like Gunicorn.


references

[JSON Web Tokens](https://learndjango.com/tutorials/django-custom-user-model)

[DRF JWT Authentication](https://github.com/wsvincent/djangox)

[Django Runserver Is Not Your Production Server](https://www.youtube.com/watch?v=eCeRC7E8Z7Y&t=59s&ab_channel=CodingWithMitch)


<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)