# Authorization/Authentication

![API](https://lh3.googleusercontent.com/proxy/2Ndo6r4AIaq4YqYvpIryvTfxEHE3rk0UTChiw4nX9h2iZTD-LFKuC_CapuA64GN-JU6fvsuCaXguMFy3CZusNNl6hUKNQtfAXrE4G6Q8b_7IGllP-upuHdx3M4bW1OugheYvWRDDsnOAz9l8eFJEtABNCfQyp-NmmaM-XaJdpStuNsoEhksOO94W1Q)

1. What header(s) are used in authentication and authorization?

 Authenticate response headers define the authentication method that should be used to gain access to a resource. They must specify which authentication scheme is used, so that the client that wishes to authorize knows how to provide the credentials.

 2. What is safe to put into a JWT?

 Only the server should know the "secret" that is used to generate the JWT. If someone modifies the data contained in the JWT, the server will fail to decode it. So the server can trust any JWT that it can decode.
However, if a hacker got access to your computer, they could see the JWT that is stored in the browser and use it. This same threat exists w/cookies, so it's not really a flaw of the JWT.
One way to mitigate this threat is the expiration date of the JWT. For a banking app, your JWT might expire after a few minutes. For Facebook, it might expire after a few months. However, there's no bullet proof solution to this if someone gets access to your browser.
Another approach for hackers would be a "man in the middle" attack to intercept the network traffic between client and server and get at the cookie/JWT. The cookie/JWT should always be sent over HTTPS to prevent this.

3. How are JWTs validated?

Check signature. The last segment of a JWT is the signature, which is used to verify that the token was signed by the sender and not altered in any way. The Signature is created using the Header and Payload segments, a signing algorithm, and a secret or public key (depending on the chosen signing algorithm).

* RBAC : Role-based access control (RBAC) is a method of restricting network access based on the roles of individual users within an enterprise. RBAC lets employees have access rights only to the information they need to do their jobs and prevents them from accessing information that doesn't pertain to them.

* User Roles :User Roles are permission sets that control access to areas and features within the Professional Archive Platform. Each User account requires a Role assignment.

* Token (JWT): SON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.