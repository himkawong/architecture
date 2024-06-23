

### Authorization Server
The Authorization Server is the Microsoft identity platform and is responsible for ensuring the user’s identity, granting and revoking access to resources, and issuing tokens. The authorization server is also known as the identity provider - it securely handles anything to do with the user’s information, their access, and the trust relationships between parties in a flow.
### The Resource Owner 
is typically the end user. It’s the party that owns the data and has the power to allow clients to access that data or resource.

### The OAuth Client
is your app, identified by its application ID. The OAuth client is usually the party that the end user interacts with, and it requests tokens from the authorization server. The client must be granted permission to access the resource by the resource owner.

### The Resource Server
is where the resource or data resides. It trusts the Authorization Server to securely authenticate and authorize the OAuth Client, and uses Bearer access tokens to ensure that access to a resource can be granted.


## Tokens

* Access Tokens
  *  tokens that a resource server receives from a client, containing permissions the client has been granted.
* ID Tokens
  * tokens that a client receives from the authorization server, used to sign in a user and get basic information about them.
* Refresh Tokens
  * used by a client to get new access and ID tokens over time. These are opaque strings, and are only understandable by the authorization server.

## Authorizaiotion Code Flow
![Authorization Code Flow](https://azure.github.io/apim-lab/assets/images/convergence-scenarios-native.svg)


[TODO]
What is the difference between OAuth and SSO ?
What is the difference betwene OAuth and OIDC ?

