# Class 15

**What is OAuth**
1. OAuth allows websites and services to share assets among users.
2. example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon.
3. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.The first site gives this token and secret to the initiating user’s client software. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site). If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website. The user approves (or their software silently approves) a particular transaction type at the first website. The user is given an approved access token (notice it’s no longer a request token). The user gives the approved access token to the first website. The first website gives the access token to the second website as proof of authentication on behalf of the user. The second website lets the first website access their site on behalf of the user.
4. OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans.

**Authorization and Authentication flows**
1. authentication is the process of verifying who a user is, while authorization is the process of verifying what they have access to.
2. exchanges an Authorization Code for a token.
3. a version of the Authorization Code Flow which makes use of a Proof Key for Code Exchange
4. the application needs only an ID token to perform user authentication.
5. authorizes the app rather than a user.
6. the device asks the user to go to a link on their computer or smartphone and authorize the device.
7. requests that users provide credentials (username and password)


**things I want to know more about**

references

[What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

[Authorization and Authentication flows](https://auth0.com/docs/get-started/authentication-and-authorization-flow)

<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)