# What is OAuth? 

‬‏ OAuth is an authentication protocol that allows you to approve one application interacting with another on your behalf without giving away your password.


---------------------





### How does OAuth work? What are the steps that it takes to authenticate the user?

How OAuth Works There are 3 main players in an OAuth transaction: the user, the consumer, and the service provider. This triumvirate has been affectionately deemed the OAuth Love Triangle.

In our example, Joe is the user, Bitly is the consumer, and Twitter is the service provided who controls Joe’s secure resource (his Twitter stream). Joe would like Bitly to be able to post shortened links to his stream. Here’s how it works:

Step 1 – The User Shows Intent

Joe (User): “Hey, Bitly, I would like you to be able to post links directly to my Twitter stream.” Bitly (Consumer): “Great! Let me go ask for permission.” Step 2 – The Consumer Gets Permission

Bitly: “I have a user that would like me to post to his stream. Can I have a request token?” Twitter (Service Provider): “Sure. Here’s a token and a secret.” The secret is used to prevent request forgery. The consumer uses the secret to sign each request so that the service provider can verify it is actually coming from the consumer application.

Step 3 – The User Is Redirected to the Service Provider

Bitly: “OK, Joe. I’m sending you over to Twitter so you can approve. Take this token with you.” Joe: “OK!”

This is the scary part. If Bitly were super-shady Evil Co. it could pop up a window that looked like Twitter but was really phishing for your username and password. Always be sure to verify that the URL you’re directed to is actually the service provider (Twitter, in this case).

Step 4 – The User Gives Permission

Joe: “Twitter, I’d like to authorize this request token that Bitly gave me.” Twitter: “OK, just to be sure, you want to authorize Bitly to do X, Y, and Z with your Twitter account?” Joe: “Yes!” Twitter: “OK, you can go back to Bitly and tell them they have permission to use their request token.” Twitter marks the request token as “good-to-go,” so when the consumer requests access, it will be accepted (so long as it’s signed using their shared secret).

Step 5 – The Consumer Obtains an Access Token

Bitly: “Twitter, can I exchange this request token for an access token?” Twitter: “Sure. Here’s your access token and secret.” Step 6 – The Consumer Accesses the Protected Resource

Bitly: “I’d like to post this link to Joe’s stream. Here’s my access token!” Twitter: “Done!” In our scenario, Joe never had to share his Twitter credentials with Bitly. He simply delegated access using OAuth in a secure manner. At any time, Joe can login to Twitter and review the access he has granted and revoke tokens for specific applications without affecting others. OAuth also allows for granular permission levels. You can give Bitly the right to post to your Twitter account, but restrict LinkedIn to read-only access.





---------------------




### What is OpenID?

OpenID is about authentication (ie. proving who you are), OAuth is about authorisation (ie. to grant access to functionality/data/etc.. without having to deal with the original authentication). OAuth could be used in external partner sites to allow access to protected data without them having to re-authenticate a user.







---------------------



### What is the difference between authorization and authentication?

Authentication, in the form of a key. The lock on the door only grants access to someone with the correct key in much the same way that a system only grants access to users who have the correct credentials. Authorization, in the form of permissions. Once inside, the person has the authorization to access the kitchen and open the cupboard that holds the pet food. The person may not have permission to go into the bedroom for a quick nap.






---------------------

### What is Authorization Code Flow?

Example The flow for authorization code is:

Create a URL to the OAuth authorization service Display the authorization user interface, prompting the user to sign in to Mendeley first if necessary Capture the authorization code from the user interface response Exchange the authorization code for an access token Extract the access token from the exchange response









---------------------




### What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

PKCE, pronounced “pixy” is an acronym for Proof Key for Code Exchange. The key difference between the PKCE flow and the standard Authorization Code flow is users aren’t required to provide a client_secret. PKCE reduces security risks for native apps, as embedded secrets aren’t required in source code, which limits exposure to reverse engineering.






---------------------


### What is Implicit Flow with Form Post?

Implicit Flow with Form Post flow uses OIDC to implement web sign-in that is very similar to the way SAML and WS-Federation operates. The web app requests and obtains tokens through the front channel, without the need for secrets or extra backend calls. With this method, you don’t need to obtain, maintain, use, and protect a secret in your application.










---------------------


### What is Client Credentials Flow?

The Client Credentials flow is a server to server flow. There is no user authentication involved in the process. In fact there is no user at all, the resulting access tokens will not contain a user, but will instead contain the Client ID as subject (if not configured otherwise).

This flow is useful for systems that need to perform API operations when no user is present. It can be nightly operations, or other that involve contacting OAuth protected APIs.

Since there is no user authorization, the flow only interacts with the Token endpoint.









---------------------






### What is Device Authorization Flow?

The OAuth 2.0 Device Authorization Grant, also known as the Device Flow, handles the scenario where user authentication is difficult to enter on the device itself. In a Device Flow, the flow is initiated by the device, but authentication is handled out-of-band on a different device with a better input, such as a browser with a keyboard for input.

The initial device polls the authorization server for a completed and successful user authentication. When it’s available, tokens are issued. The Device Flow is a useful authorization flow commonly used with smart TVs and devices like Apple TV.

The OAuth Device Flow article describes the mechanics of the flow. In this tutorial, we will outline how to set it up in the Curity Identity Server.






---------------------

### What is Resource Owner Password Flow?

The Resource Owner Password Credentials flow allows exchanging the username and password of a user for an access token and, optionally, a refresh token. This flow has significantly different security properties than the other OAuth flows. The primary difference is that the user’s password is accessible to the application. This requires strong trust of the application by the user.















