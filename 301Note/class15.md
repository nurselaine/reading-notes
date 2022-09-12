## Reading NOtes Class 15: Authentication

#### What is OAuth

1. What is OAuth?
  - open-standard authorization protocol/framework for servers and services to authenticate users without needing the inital logon credential aka secure, third-part, user-agent delegated authorization
  - think of OAuth as AUTHorization
2. Give an example of what using OAuth would look like.
  - logging into a website and it has 1_ chances to log on using another website's logon information. Instead of the website you are currently on authenticating your information, the other website you agree to share your logon information will validate your informaiton 
  - to get permission to access one website by using another website's validation 
  - 1+ services are being used for one transaction by the client/user to reduce the amount of times a user is asked to sign in
3. How does OAuth work? What are the steps that it takes to authenticate the user?
  - Using another service's authentication of the user's identity, Oauth allows the user's service to authorize access once the user has allowed Oauth on the client side
  1. first website connects to second website on behalf of user
  2. second site creates unique token and ?secret unique
  3. first site gives token and secret to transaction & parties involved
  4. information is provided to authorization provider (doesn't have to be second site)
  5. once authenicated, client is asked to approve authorization transaction to second site on the first site aka software silently approves
  6. user is given approved access token which is then used on the first site to pass to the second site as proof of authentication
  7. second site now has authentication token which allows first site access to their site then a successful transaction occurs
  - kerberos works similarly to Oauth
4. What is OpenID?
  - authentication - humans logging into machines vs machines logging into machines which is what Oauth does
  - single sign-in to authenticate identities of users
  - openID is now an authentication layer for Oauth

#### Authorization and Authentication flows

1. What is the difference between authorization and authentication?
  - authentication is the process of a user proving ownership through a given identity
  - authorization is the process of letting a user access resources after a successful authentication
2. What is Authorization Code Flow?
  - for web apps to exchange authorization codes for tokens
3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
  - additional information is needed when using mobile and native applications aka a proof key code which is supported to OAuth
4. What is Implicit Flow with Form Post?
  - for applications unable to securely store client secrets, it utilizes a form post to request authentication via ID token
5. What is Client Credentials Flow? 
  - used for authentication and authorization with server side systems where usernames and passwords don't matter, but a client credential will
6. What is Device Authorization Flow?
  - some devices have input constraints that require user to go to a link on a device and authorize the device to avoid poor user experience 
7. What is Resource Owner Password Flow?
  - applications that request users provide username and password using a form 

  what's a good project to practice all of these authentication methods

**Videos**
###### Auth0 for single page apps