---
api_key_in: []
auth_types:
- saml2
- openid-connect
- ldap
- directory
- password
description: ''
kind: authentication
layout: security
method: searched
name: Aryaka Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aryaka secures its APIs with saml2, openid-connect, ldap, directory, and password across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aryaka
provider_slug: aryaka
scheme_count: 3
schemes:
- backends:
  - docs: https://docs.aryaka.com/space/KNOW/1091371017/Configure+AIM+for+Aryaka's+IdP
    name: Aryaka's IdP
  - docs: https://docs.aryaka.com/space/KNOW/1090388026/Configure+AIM+for+Active+Directory
    name: Active Directory
  - docs: https://docs.aryaka.com/space/KNOW/1090191369/Configure+AIM+for+LDAP
    name: LDAP
  - docs: https://docs.aryaka.com/space/KNOW/203325458/Configure+Microsoft+Entra+for+AIM
    name: Microsoft Entra ID (SAML)
  - docs: https://docs.aryaka.com/space/KNOW/144638068/Configure+Okta+SAML+for+AIM
    name: Okta (SAML)
  - docs: https://docs.aryaka.com/space/KNOW/277381162/Configure+Cisco+Duo+for+AIM
    name: Cisco Duo (SAML/MFA)
  description: AIM is Aryaka's identity layer for portal and network-user authentication. It can federate to an external IdP or use Aryaka's own IdP.
  name: Aryaka Identity Management (AIM)
  sources:
  - docs.aryaka.com
  type: identity-provider-integration
- description: SAML 2.0 single sign-on into the MyAryaka portal, configurable against Azure AD/Entra and Okta. OIDC is supported through the Okta integration catalog listing.
  docs:
  - https://docs.aryaka.com/space/KNOW/862388286/Configure+SSO
  - https://docs.aryaka.com/space/KNOW/862486592/Log+in+to+MyAryaka+using+SSO
  - https://docs.aryaka.com/space/KNOW/1268613131/Configure+SSO+with+Azure+AD
  - https://docs.aryaka.com/space/KNOW/1268809736/Configure+SSO+with+Okta
  login_url: https://my.aryaka.com/
  name: MyAryaka portal SSO
  sources:
  - docs.aryaka.com
  type: saml2
- description: SSO and delegated access control for "Powered by Aryaka" partners and MSPs.
  docs:
  - https://docs.aryaka.com/space/PTNR/784072990/Configure+partner+SSO
  - https://docs.aryaka.com/space/PTNR/784597057/Manage+access+control
  login_url: https://aryaka.my.site.com/partnercommunity/CommunityLogin
  name: MyAryaka Partner Portal SSO
  sources:
  - docs.aryaka.com
  type: saml2
slug: aryaka-authentication
source_filename: aryaka-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://docs.aryaka.com/space/KNOW/1510247/Aryaka+Identity+Management\ndocs: https://docs.aryaka.com/space/KNOW/862388286/Configure+SSO\nscope: platform-and-portal\nnote: >-\n  SCOPE MATTERS: Aryaka publishes no public API, so there are no OpenAPI securitySchemes\n  to derive from and nothing here describes API authorization. What Aryaka does document\n  in depth is Aryaka Identity Management (AIM) — the identity, SSO and role-based access\n  control model for the MyAryaka customer portal and the MyAryaka Partner Portal, plus\n  the network-user identity model used by the security engines. That is what this profile\n  records. There is no documented API key, bearer token, or OAuth client-credentials\n  surface for programmatic access; scopes/ is therefore intentionally absent.\nsummary:\n  types: [saml2, openid-connect, ldap, directory, password]\n  api_key_in: []\n  oauth2_flows: []\n  api_authentication: none-published\n\
  schemes:\n- name: Aryaka Identity Management (AIM)\n  type: identity-provider-integration\n  description: >-\n    AIM is Aryaka's identity layer for portal and network-user authentication. It can\n    federate to an external IdP or use Aryaka's own IdP.\n  backends:\n  - {name: \"Aryaka's IdP\", docs: \"https://docs.aryaka.com/space/KNOW/1091371017/Configure+AIM+for+Aryaka's+IdP\"}\n  - {name: Active Directory, docs: 'https://docs.aryaka.com/space/KNOW/1090388026/Configure+AIM+for+Active+Directory'}\n  - {name: LDAP, docs: 'https://docs.aryaka.com/space/KNOW/1090191369/Configure+AIM+for+LDAP'}\n  - {name: Microsoft Entra ID (SAML), docs: 'https://docs.aryaka.com/space/KNOW/203325458/Configure+Microsoft+Entra+for+AIM'}\n  - {name: Okta (SAML), docs: 'https://docs.aryaka.com/space/KNOW/144638068/Configure+Okta+SAML+for+AIM'}\n  - {name: Cisco Duo (SAML/MFA), docs: 'https://docs.aryaka.com/space/KNOW/277381162/Configure+Cisco+Duo+for+AIM'}\n  sources: [docs.aryaka.com]\n- name: MyAryaka portal\
  \ SSO\n  type: saml2\n  description: >-\n    SAML 2.0 single sign-on into the MyAryaka portal, configurable against Azure AD/Entra\n    and Okta. OIDC is supported through the Okta integration catalog listing.\n  login_url: https://my.aryaka.com/\n  docs:\n  - https://docs.aryaka.com/space/KNOW/862388286/Configure+SSO\n  - https://docs.aryaka.com/space/KNOW/862486592/Log+in+to+MyAryaka+using+SSO\n  - https://docs.aryaka.com/space/KNOW/1268613131/Configure+SSO+with+Azure+AD\n  - https://docs.aryaka.com/space/KNOW/1268809736/Configure+SSO+with+Okta\n  sources: [docs.aryaka.com]\n- name: MyAryaka Partner Portal SSO\n  type: saml2\n  description: SSO and delegated access control for \"Powered by Aryaka\" partners and MSPs.\n  login_url: https://aryaka.my.site.com/partnercommunity/CommunityLogin\n  docs:\n  - https://docs.aryaka.com/space/PTNR/784072990/Configure+partner+SSO\n  - https://docs.aryaka.com/space/PTNR/784597057/Manage+access+control\n  sources: [docs.aryaka.com]\nauthorization:\n\
  \  model: role-based-access-control\n  description: >-\n    Roles, user groups and users are managed per customer and per partner tenant, with\n    importable role definitions and a documented RBAC FAQ. Partner tenants carry a\n    separate role/user/group surface over their downstream customers.\n  docs:\n  - https://docs.aryaka.com/space/KNOW/774242406/Access+Control+overview\n  - https://docs.aryaka.com/space/KNOW/774438999/Add,+edit,+and+delete+roles\n  - https://docs.aryaka.com/space/KNOW/1269170384/FAQ:+How+do+I+implement+role-based+access+control?\nnetwork_user_identity:\n  description: >-\n    A separate identity surface: mapping network users to identities so ZTNA, SWG, CASB\n    and SaaS-application access-control policies can be written against users and groups.\n  docs: https://docs.aryaka.com/space/KNOW/1272545378/Network+user+identity+management\nabsences:\n  api_keys: not-published\n  bearer_tokens: not-published\n  oauth2: not-published\n  mutual_tls: not-published\n  openid_connect_discovery:\
  \ 'no /.well-known/openid-configuration served on any Aryaka host'\nx-evidence:\n  fetched: '2026-08-02'\n  method: docs sitemap enumeration + live HTTP probes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aryaka/refs/heads/main/authentication/aryaka-authentication.yml
summary_line: saml2/openid-connect/ldap/directory/password · 3 schemes
tags:
- Company
- Networking
- SASE
- SD-WAN
- Network Security
- Zero Trust
- ZTNA
- Cloud Connectivity
- Managed Service
- Firewall
- Secure Web Gateway
- WAN Optimization
- Multi-Cloud
- Telecommunications
---
