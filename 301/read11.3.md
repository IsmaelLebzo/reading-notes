# Authentication

![image](https://i.ytimg.com/vi/CPbvxxslDTU/maxresdefault.jpg)

## What is OAuth?

OAuth allows users to transfer assets between websites and services. Although it is commonly accepted, be mindful of its flaws.

Providing a seamless, single sign-on (SSO) access experience among multiple computers, each of which requires unrelated logon accounts to access their services and content, has been one of the most difficult computer security nuts to crack since the beginning of distributed personal computer networks.

## OAuth definition

OAuth is an open-standard authorization protocol or framework that explains how unconnected servers and services may properly enable authorized access to their assets without having to share a single login credential. This is referred to as secure, third-party, user-agent, delegated authorisation in authentication jargon.

## OAuth history

OAuth was created and heavily backed by Twitter, Google, and other corporations from the start, and it was issued as an open standard in 2010 as RFC 5849, and it soon gained widespread use. Over the next two years, it was extensively revised, and version 2.0 of OAuth was published as RFC 6749 in 2012. Even though version 2.0 was severely panned for a variety of reasons, including those listed below, it grew in popularity. Amazon, Facebook, Instagram, LinkedIn, Microsoft, Netflix, Paypal, and a slew of other digital heavyweights have all signed on as early adopters.

## OAuth examples

The most basic example of OAuth is when you attempt to connect onto a website and it gives one or more options to log on using the login credentials of another website or service. You then click the link to the other website, which authenticates you, and the website you were originally connecting to logs you on using the authorization granted by the second website.

## OAuth explained

When learning about OAuth, keep in mind that most OAuth instances involve two unconnected sites or services attempting to do something on behalf of users or their software. For the final transaction to be allowed, all three must collaborate and get numerous approvals.

## How OAuth works

Assume that a user has already joined up for a website or service (OAuth only works using HTTPS). The user then launches a feature/transaction that requires access to a separate site or service.

# Authentication and Authorization Flows

Auth0 authenticates users and obtains their authorisation to access protected resources using the OpenID Connect (OIDC) Protocol and the OAuth 2.0 Authorization Framework. Without worrying about OIDC/OAuth 2.0 requirements or other technical elements of authentication and authorization, you can simply handle multiple flows in your own apps and APIs using Auth0.

## Authorization Code Flow

Regular web apps may utilize the Authorization Code Flow, which trades an Authorization Code for a token, because they are server-side programs with no publicly accessible source code.

- Authorization Code Flow

- Add Login Using the Authorization Code Flow

- Call API Using the Authorization Code Flow

## Implicit Flow with Form Post

The Implicit Flow is an alternative to the Authorization Code Flow that is designed for Public Clients or applications that are unable to securely hold Client Secrets. While this is no longer considered a best practice for requesting Access Tokens, it does provide a simplified workflow when combined with Form Post response mode if the application just requires an ID token for user authentication.

## Hybrid Flow

The Hybrid Flow, which combines features of the Authorization Code Flow and Implicit Flow with Form Post to allow your application to have immediate access to an ID token while still providing secure and safe retrieval of access and refresh tokens, may benefit applications that are able to securely store Client Secrets. This is beneficial in cases when your program wants to obtain information about the user right away, but first has to process certain data before getting access to protected resources for a long period of time.

## Device Authorization Flow

Instead of immediately authenticating the user, input-constrained devices that connect to the internet ask the user to go to a URL on their computer or smartphone and approve the device. This prevents users from having a bad experience on devices that don't have a simple way to enter text. Device apps utilize the Device Authorization Flow to do this (drafted in OAuth 2.0). For usage with mobile and native apps.

