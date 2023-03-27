### Adam Strickland (adamstrickland97@gmail.com)
Technical problem solver with expertise in web and native app security and networking protocols. Technologies I know:
- [RESTful web services](#restful-web-services) and HTTP
- [Session management](#session-management) using cookies, tokens, or certificates
- [Applied cryptography](#applied-cryptography), for example JWTs
- [Authentication systems](#authentication-systems) and chains of trust, for example OAuth 2.0, OIDC and FIDO/WebAuthn
- [Cross-Site request forgery](#csrf-protection) (CSRF) protection

I like to say that if it uses HTTP, I can hack it! I can quickly examine a network trace (for example, using Burp Suite) and understand how a web or native application ticks.

<!--
**madaster97/madaster97** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

### My Work
#### RESTful Web Services
- [Updated](https://github.com/cds-hooks/api/pull/5) the Swagger/OpenAPI spec for the CDS Hooks REST API
- [Implemented](https://github.com/madaster97/puri-fhir) an example CDS Hooks service for my company's use in demos (hosted in pipedream)

#### Session Management
- [Discovered and fixed](https://github.com/auth0/express-openid-connect/pull/188) an issue with an Openid Connect library, where sessions didn't work embedded in an iframe
- [Added testing](https://github.com/sgpinkus/express-session/pull/1) for a feature of the express-session library

#### Applied Cryptography
- [Demonstrated](https://github.com/madaster97/openssl-jws) how to sign Elliptic-Curve JWTs with the openssl CLI
- [Contributed](https://github.com/auth0/express-openid-connect/pull/291) JWT authentication functionality to an Openid Connect library

#### Authentication Systems
- [Contributed](https://github.com/tavrez/openssh-sk-winhello/pull/16) to a FIDO/WebAuthn library that brighes OpenSSH with Windows Hello
- Identified a broken authentication issue in one of my company's integrations. I used my knowledge of crpytography to exploit an encryption system

#### CSRF Protection
- Identified a login CSRF attack at my company, and prevented us from pushing the code to production
- Had a [throrough conversation](https://github.com/auth0/express-openid-connect/issues/426) with Openid Connect library maintainers on the scope of CSRF attacks against the library (Planning a PR to add [documentation](https://github.com/madaster97/express-openid-connect/blob/addl-csrf-docs/EXAMPLES.md#11-use-sdk-session-for-csrf-protection) on edge cases)
