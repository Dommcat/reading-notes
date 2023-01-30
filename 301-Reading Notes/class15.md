# 301 Reading Notes

## Class 15 Summary: This class reading is about Authentication

What is OAuth?
-OAuth is an open-standard authorization protocol or framework

Give an example of what using OAuth would look like.
-when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon.

How does OAuth work? What are the steps that it takes to authenticate the user?
-(OAuth only works using HTTPS). The user then initiates a feature/transaction that needs to access another unrelated site or service. The following happens (greatly simplified):

What is OpenID?

- OpenID is about authentication

as a commenter on StackOverflow pithily put it: "OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans.

Source: <https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html>

What is the difference between authorization and authentication?
-"OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans.

Source: <https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html>

What is Authorization Code Flow?
-Because regular web apps are server-side apps where the source code is not publicly exposed, they can use the Authorization Code Flow  which exchanges an Authorization Code for a token.

What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
-During authentication, mobile and native applications can use the Authorization Code Flow, but they require additional security.

What is Implicit Flow with Form Post?
-As an alternative to the Authorization Code Flow, OAuth 2.0 provides the Implicit Flow, which is intended for Public Clients, or applications which are unable to securely store Client Secrets.

What is Client Credentials Flow?
-With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user.

What is Device Authorization Flow?
-With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device.

What is Resource Owner Password Flow?
-Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form.

## Things I want to know more about
