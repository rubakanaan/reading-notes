## What is OAuth?
"Open standard authorization protocol or framework" What does this mean? It means that sites that have nothing to do with eachother can use the same standard of authorization to make is easier on the user.
<br>

## Give an example of what using OAuth would look like.
An example would be when one goes to a site and sees things like 'Log in with Facebook' or 'Log in using Google.' These let a user not have to make a new login for the site.
<br>

## How does OAuth work? What are the steps that it takes to authenticate the user?
Website the user is visiting connects to the one that holds their authentication information --> this site with the user's information generates a token to provide --> this token is provided to the site the user visited --> client may be asked to authenticate --> client is asked to approve authorization transaction --> user is given approved access token which then goes to the original site --> proof of the authentication is given to the second site --> user sees the transaction happening on the screen
<br>

## What is OpenID?
OpenID is an authenticator that was a competitor to Facebook connect, but didn't have the same name recognition, and has now been reinvented as an authentication aprt of OAuth.
<br>

# Authorization & Authentication 

## What is the difference between authorization and authentication?
**Authentication:** Verifying who user is Authorization: Verifying what user can access

An example: when one buys alcohol at the store, you must show your photo ID to verify your age. Them scanning the ID would be authentication. Authorization would be them pressing a button or typing into their computer that the transaction can be carried on with.
<br>

## What is Authorization Code Flow?
Exchanges an Authorization Code for a token. The app has to be server side.

- User attempt so log in
- User is redirected ti Auth0 Server
- Auth0 redirects to authorization prompt
- User authenticates and gives appropriate permissions to new site
- Auth0 redirects user to application with an one-time authorization code
- This code is sent to a different endpoint in ths server, with the information about the client
- Auth0 Authorization verifies information
- Auth0 responds with ID and Access Tokens
- App uses access token to get info about user

<br>

## What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
**PKCE** = Proof Key for Code Exchange

For this PKCE, when a user attempt to log in, there is a random code that is generated. The user then is redirected to the Auth0 server, then redirected to the login. Permissions page is then shown, and they authenticate, then user is redirected to the app. The next steps are the same as for a non-PKCE flow.
<br>

## What is Implicit Flow with Form Post?
- User clicks login button
- Auth0 redirects to server, passing id token, and form post.
- Auth0 server redirects user to login prompt
- User authenticates and is shown permissions options
- Auth0 server redirects user back to app with the ID token
<br>

## What is Client Credentials Flow?
It is for authorizing not users with a name and password, but applications.
<br>
Flow = app authenticated with Auth0 server --> Auth0 validated Client ID and Secret --> responds with access token --> token is used to call on APIs
<br>

## What is Device Authorization Flow?
Device authorization flow is used to provide a better experience for devices that don't have an easy way to enter text, like a TV streaming service.
<br>

## What is Resource Owner Password Flow?
This is generally not preferred when compared to redirect authentication methods, but can be used with trusted applications. It usualy comes in the username/password format. Users credentials are directly given to the server.