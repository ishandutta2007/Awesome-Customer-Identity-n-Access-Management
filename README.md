# Awesome-Customer-Identity-n-Access-Management

# Top Customer Identity & Access Management (CIAM) Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Customer Authentication, Multi-Tenancy, SSO & User Management*
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Customer Identity & Access Management (CIAM)**. These tools help organizations authenticate and manage customer identities across applications, providing secure login, registration, social sign-on, and multi-tenant organization management.

**Examples** include Auth0, Okta Customer Identity, Amazon Cognito, FusionAuth, Descope, WorkOS, Stytch, LoginRadius, PingOne for Customers, and SuperTokens (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom authentication flows, and transparent identity data — ideal for organizations that need full control over customer identity without per-MAU SaaS fees or vendor lock-in.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Auth0](https://auth0.com/)**  
  The dominant CIAM platform. Provides authentication, authorization, social login, MFA, and extensibility via Actions/Rules. Enterprise-grade with extensive SDKs and integrations.

- **[Okta Customer Identity](https://www.okta.com/)**  
  Enterprise CIAM solution within Okta's broader identity platform. Provides authentication, MFA, and user management for customer-facing applications.

- **[Amazon Cognito](https://aws.amazon.com/cognito/)**  
  AWS-native CIAM service. Provides user pools for authentication and identity pools for AWS credential federation, integrated with the AWS ecosystem.

- **[Descope](https://www.descope.com/)**  
  No-code CIAM platform with visual workflow builder. Provides passwordless authentication, MFA, and user management with drag-and-drop orchestration.

- **[WorkOS](https://workos.com/)**  
  Enterprise-ready CIAM focused on SSO and directory sync. Provides APIs for adding enterprise SSO (SAML, OIDC) and SCIM provisioning to existing applications.

- **[Stytch](https://stytch.com/)**  
  Developer-first authentication platform. Provides passwordless login, MFA, and session management with strong API design.

- **[LoginRadius](https://www.loginradius.com/)**  
  CIAM platform with social login, MFA, and user management. Provides identity APIs and compliance features.

- **[PingOne for Customers](https://www.pingidentity.com/)**  
  Enterprise CIAM solution within Ping Identity's platform. Provides authentication, authorization, and identity orchestration for customer applications.

- **[FusionAuth](https://fusionauth.io/)**  
  Developer-focused CIAM platform. Offers a **free Community Edition** for self-hosting with unlimited MAU. Provides authentication, SSO, social login, and MFA with extensive APIs .

- **[SuperTokens](https://supertokens.com/)**  
  Open-core authentication platform. Provides embedded login UI and session management with Apache 2.0 core. **Note**: Auth0 embedded alternative; SAML SSO requires paid tier .

## Open-Source GitHub Projects

### Full-Featured CIAM Platforms

- **[Keycloak](https://github.com/keycloak/keycloak)**  
  **The most mature and widely adopted open-source identity platform.** **Apache-2.0 licensed**, developed by Red Hat and a **CNCF project** . Provides comprehensive SSO, social login, MFA, LDAP/Active Directory federation, and user federation. Admin console for centralized management, clustering for high availability, and extensive plugin ecosystem. **Best for**: Enterprise-grade CIAM with broad protocol coverage (OIDC, OAuth 2.0, SAML 2.0) and directory federation .

- **[Zitadel](https://github.com/zitadel/zitadel)**  
  **Modern CIAM built for B2B SaaS and multi-tenancy.** **AGPL-3.0 licensed** (with SDK carve-outs). Native multi-tenant architecture with organizations and projects as first-class concepts. Event-sourced for full audit trail of permission changes. Supports OAuth 2.0, OIDC, SAML 2.0, SCIM, FIDO2, and passkeys. **Best for**: B2B SaaS requiring native multi-tenancy and organization isolation .

- **[Ory (Kratos / Hydra / Keto)](https://github.com/ory/kratos)**  
  **Cloud-native, API-first, headless identity stack.** **Apache-2.0 licensed**. Modular components: **Kratos** (identity management), **Hydra** (OAuth2/OIDC), **Keto** (Zanzibar-inspired authorization), **Polis** (SAML), **Oathkeeper** (identity proxy). Designed for Kubernetes with independent scaling. **Best for**: Teams wanting complete UI freedom and composable, headless architecture .

- **[Authentik](https://github.com/goauthentik/authentik)**  
  **User-friendly open-source identity provider.** Focuses on usability while offering powerful capabilities. Supports SAML, OAuth2, LDAP, RADIUS, and more. Features application proxy for adding SSO to legacy apps. Docker-based deployment. **Best for**: Smaller teams wanting a single, approachable product .

- **[Casdoor](https://github.com/casdoor/casdoor)**  
  **Open-source identity and access management platform with a modern UI.** Go-based, supports OAuth 2.0, OIDC, SAML, LDAP, and CAS. Provides extensive SDKs and examples across languages and frameworks. **Best for**: Teams wanting a UI-first IAM with broad protocol support .

- **[Idenplane](https://github.com/idenplane/idenplane)**  
  **Lightweight CIAM alternative to Keycloak and Auth0.** **TypeScript/NestJS with PostgreSQL**, runs in **~150 MB RAM** (vs Keycloak's 1 GB+). Supports OAuth 2.0, OIDC, SAML 2.0, WebAuthn/FIDO2, TOTP/MFA, and SCIM 2.0. Features multi-tenancy via realms, organizations (B2B), RBAC + ABAC, and adaptive auth (risk-based step-up, impossible-travel detection) .

### Developer-Focused Authentication

- **[SuperTokens](https://github.com/supertokens/supertokens-core)**  
  **Open-source authentication with embedded login UI and session management.** **Apache-2.0 licensed** core with unlimited MAU. User data and password hashes stored in your own PostgreSQL/MySQL. Provides email/password, social login, passwordless, and secure session management with rotating refresh tokens. **Best for**: Product teams wanting to own the auth code path without running a full IAM server .

- **[Stack Auth](https://github.com/stack-auth/stack)**  
  **Developer-friendly, fully open-source authentication for Next.js and React.** **MIT and AGPL licensed**. Provides pre-built `<SignIn/>` and `<SignUp/>` components, OAuth, password credentials, magic links, and passkeys. Includes user dashboard, account settings, multi-tenancy with organizations, and RBAC. **Best for**: Next.js/React teams wanting a 5-minute setup with managed service optionality .

- **[Hanko](https://github.com/teamhanko/hanko)**  
  **Open-source authentication and user management for the passkey era.** Supports passkeys, social logins, SAML SSO, and MFA. Provides embeddable web components (`<hanko-auth>`) for login/registration. API-first, small footprint, cloud-native. **Best for**: Teams wanting passkey-first authentication with embeddable UI .

- **[LoginLink](https://github.com/websvcin/loginlink)**  
  **Self-hosted OAuth 2.0 + OIDC identity platform for multi-tenant SaaS.** **.NET 8** with **one SQLite database per tenant** for complete isolation. Supports password (Argon2id), Google/GitHub/Microsoft/Apple OAuth, Email/SMS OTP, TOTP, WebAuthn/Passkeys, Magic Link, and SAML. Management REST API + SCIM. **Best for**: Multi-tenant SaaS wanting per-tenant data isolation .

- **[Authelia](https://github.com/authelia/authelia)**  
  **Lightweight authentication and authorization server for protecting internal tools.** **Apache-2.0 licensed**, deploys as a single container. Adds TOTP, WebAuthn/passkeys, and Duo push MFA in front of apps that don't natively support them. **Best for**: Protecting internal tools and self-hosted services, not customer-facing SaaS login .

### Enterprise & Federation

- **[WSO2 Identity Server](https://github.com/wso2/product-is)**  
  **Market-leading open-source CIAM solution.** Manages **over one billion identities** for **250+ customers** in financial services, healthcare, government, and retail . Provides SSO, MFA, user provisioning, access certification, and unified directory. Available as IDaaS, installable software, or private cloud . **Best for**: Large enterprises with complex CIAM requirements and compliance needs.

- **[Perun](https://github.com/CESNET/Perun)**  
  **Identity and access management for distributed and federated environments.** **FreeBSD licensed**, developed by CESNET and Masaryk University. Focuses on **virtual organization (VO) management**, group management, and resource management. Supports SAML2, LDAP, and various authentication protocols. **Best for**: Research and academic federated identity management .

### Additional Strong Open-Source Options

- **Full CIAM Platforms**: **Keycloak** (CNCF, Apache-2.0, enterprise-grade) , **Zitadel** (AGPL-3.0, B2B multi-tenant) , **Ory** (Apache-2.0, headless/composable) , **Authentik** (user-friendly, single product) , **Casdoor** (modern UI, broad SDKs) , **Idenplane** (lightweight, TypeScript) .
- **Developer-Focused**: **SuperTokens** (embedded UI, Apache-2.0 core) , **Stack Auth** (Next.js/React, MIT/AGPL) , **Hanko** (passkey-first, embeddable) , **LoginLink** (.NET, per-tenant isolation) .
- **Enterprise/Federation**: **WSO2 Identity Server** (1B+ identities) , **Perun** (research federation, FreeBSD) .
- **Internal Tools**: **Authelia** (lightweight, single container) .

**Frameworks for building custom systems**: Combine **Keycloak** for enterprise-grade CIAM with broad protocol coverage, **Zitadel** for B2B multi-tenant SaaS, **Ory** for headless/composable architecture with full UI control, **SuperTokens** or **Stack Auth** for embedded in-app authentication, and **Hanko** for passkey-first experiences. Add **PostgreSQL** for persistence and **Docker/Kubernetes** for deployment.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- CIAM platforms handle sensitive customer identity and authentication data; ensure compliance with GDPR, CCPA, and relevant data protection regulations.
- **Open-source reality**: The open-source ecosystem for CIAM is **mature and production-proven**. **Keycloak** is the broadest open-source IdP with enterprise adoption and CNCF backing . **Zitadel** provides modern B2B multi-tenancy with event sourcing . **Ory** delivers composable, headless identity for cloud-native architectures . **SuperTokens** and **Stack Auth** offer developer-friendly embedded authentication . **WSO2 Identity Server** manages over a billion identities for enterprise customers . However, **commercial platforms** (Auth0, Okta, Descope, WorkOS) provide **managed infrastructure, SLA-backed support, and enterprise features** that open-source alternatives require significant operational investment to match. The open-source path is **genuinely viable** for organizations with strong identity engineering capacity.

---

**Made for security engineers, platform teams, full-stack developers, and identity architects.**
Let's make customer identity and access management more open, transparent, and developer-friendly.
