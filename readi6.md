# Bearer Authorization

![API](https://nordicapis.com/wp-content/uploads/Building-a-RESTful-API-Using-Node.JS-and-MongoDB.png)


1. Write the following steps in the correct order:
Receive access token
Redirect to a third party authentication endpoint
Register your application to get a client_id and client_secret
Make a request to a third-party API endpoint
Ask the client if they want to sign in via a third party
Receive authorization code
Make a request to the access token endpoint

2. What can you do with an authorization code?

client will get back with the auth code and client credentials will request for a token.
3. What can you do with an access token?

Will it can be used as a applications use to make API requests on behalf of a user.
4. What’s a benefit of using OAuth instead of your own basic authentication?

It allows you to read data of a user from another application.
It supplies the authorization workflow for web, desktop applications, and mobile devices.
Is a server side web app that uses authorization code and does not interact with user credentials.

* JWTs Explained : JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.
 
* Here are some scenarios where JSON Web Tokens are useful:

Authorization: This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.

Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally, as the signature is calculated using the header and the payload, you can also verify that the content hasn't been tampered with

* Are JWTs Secure?
WTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore.

Answer to your comment: I'm not sure if I understand your comment the right way. Just to be sure: do you know and understand digital signatures? I'll just briefly explain one variant (HMAC, which is symmetrical, but there are many others).

Let's assume Alice wants to send a JWT to Bob. They both know some shared secret. Mallory doesn't know that secret, but wants to interfere and change the JWT. To prevent that, Alice calculates Hash(payload + secret) and appends this as signature.

When receiving the message, Bob can also calculate Hash(payload + secret) to check whether the signature matches. If however, Mallory changes something in the content, she isn't able to calculate the matching signature (which would be Hash(newContent + secret)). She doesn't know the secret and has no way of finding it out. This means if she changes something, the signature won't match anymore, and Bob will simply not accept the JWT anymore.

Let's suppose, I send another person the message {"id":1} and sign it with Hash(content + secret). (+ is just concatenation here). I use the SHA256 Hash function, and the signature I get is: 330e7b0775561c6e95797d4dd306a150046e239986f0a1373230fda0235bda8c. Now it's your turn: play the role of Mallory and try to sign the message {"id":2}. You can't because you don't know which secret I used. If I suppose that the recipient knows the secret, he CAN calculate the signature of any message and check if it's correct.