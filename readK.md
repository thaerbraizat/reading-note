# Authentication
![react](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

1. What is OAuth?

OAuth is an open standard for access delegation, commonly used as a way for Internet users to grant websites or applications access to their information on other websites but without giving them the passwords

2. Give an example of what using OAuth would look like?

The simplest example of OAuth in action is one website saying “hey, do you want to log into our website with other website's login?” In this scenario, the only thing the first website – let's refer to that website as the consumer – wants to know is that the user is the same user on both websites and has logged in 

3. How does OAuth work? What are the steps that it takes to authenticate the user?

* The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
* The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
* The first site gives this token and secret to the initiating user’s client software.
* The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
* If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the
 second website.
* The user approves (or their software silently approves) a particular transaction type at the first website.
* The user is given an approved access token (notice it’s no longer a request token).
* The user gives the approved access token to the first website.
* The first website gives the access token to the second website as proof of authentication on behalf of the user.
* The second website lets the first website access their site on behalf of the user.
* The user sees a successfully completed transaction occurring.
* **OAuth** is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

4. What is OpenID?

OpenID is an open standard and decentralized authentication protocol. Promoted by the non-profit OpenID Foundation, it allows users to be authenticated by cooperating sites using a third-party service

##  Authorization and Authentication flows

1. What is the difference between authorization and authentication?

Authentication :telling the system who you are by providing username and password
Authorization  :things you can do according to who you are 
 
2. What is Authorization Code Flow?

Authorization code flow is used to obtain an access token to authorize API requests. ... Access tokens, obtained using authorization code flow, provide permissions for your application to manipulate documents and other resources on behalf of a Mendeley user and make requests for all API resources.

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

The Authorization Code Flow + PKCE is an OpenId Connect flow specifically designed to authenticate native or mobile application users. This flow is considered best practice when using Single Page Apps (SPA) or Mobile Apps. PKCE, pronounced **pixy** is an acronym for Proof Key for Code Exchange.

4. What is Implicit Flow with Form Post?

Implicit Flow with Form Post flow uses OIDC to implement web sign-in that is very similar to the way SAML and WS-Federation operates. The web app requests and obtains tokens through the front channel, without the need for secrets or extra backend calls.

5. What is Client Credentials Flow?

The Client Credentials flow is a server to server flow. There is no user authentication involved in the process. ... This flow is useful for systems that need to perform API operations when no user is present. It can be nightly operations, or other that involve contacting OAuth protected APIs.

6. What is Device Authorization Flow?

The OAuth 2.0 Device Authorization Grant (formerly known as the Device Flow) is an OAuth 2.0 extension that enables devices with no browser or limited input capability to obtain an access token. This is commonly seen on Apple TV apps, or devices like hardware encoders that can stream video to a YouTube channel.

7. What is Resource Owner Password Flow?

The Resource Owner Password Credentials flow allows exchanging the username and password of a user for an access token and, optionally, a refresh token. The primary difference is that the user's password is accessible to the application..

## Things I want to know more about


### Resource
* [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html).
* [Authorization and Authentication flows](https://auth0.com/docs/flows).



