---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Onestream Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: OneStream secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: OneStream
provider_slug: onestream
scheme_count: 2
schemes:
- bearerFormat: PAT
  description: 'Personal Access Token generated in the OneStream Identity & Access Management portal (IdentityServer). Works with native auth and any OIDC or SAML 2.0 compliant external identity provider. Sent as `Authorization: Bearer <token>`.'
  name: PersonalAccessToken
  scheme: bearer
  source: https://documentation.onestream.com/1375907/Content/IDM/OneStream%20IdentityServer.html
  type: http
- description: OAuth 2.0 client_credentials grant for self-hosted environments federating to a supported external provider (Microsoft Entra ID / Azure AD, Okta, PingFederate). Requires Client ID, Client Secret, and the provider Token URL; the returned access token is used as a bearer token on API calls.
  flows:
  - flow: clientCredentials
    scopes: {}
    tokenUrl: provider-specific (Azure AD / Okta / PingFederate token endpoint)
  name: OAuth2ClientCredentials
  source: https://documentation.onestream.com/docs/Content/REST%20API/Configure%20OneStream%20API%20for%20External.html
  type: oauth2
slug: onestream-authentication
source_filename: onestream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://documentation.onestream.com/docs/Content/REST%20API/Authentication2.html\ndocs:\n- https://documentation.onestream.com/docs/Content/REST%20API/Authentication2.html\n- https://documentation.onestream.com/docs/Content/REST%20API/Configure%20OneStream%20API%20for%20External.html\n- https://documentation.onestream.com/1375907/Content/IDM/OneStream%20IdentityServer.html\nsummary:\n  types:\n  - oauth2\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    OneStream secures its REST (Web) API with bearer tokens. Cloud tenants on\n    OneStream IdentityServer issue Personal Access Tokens (PATs) managed in the\n    Identity & Access Management portal. Self-hosted deployments federate to an\n    external identity provider (Microsoft Entra ID / Azure AD, Okta, or\n    PingFederate) using the OAuth 2.0 client_credentials grant. Access tokens\n    are presented on every request as `Authorization:\
  \ Bearer <token>`.\nschemes:\n- name: PersonalAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: PAT\n  description: >-\n    Personal Access Token generated in the OneStream Identity & Access\n    Management portal (IdentityServer). Works with native auth and any OIDC or\n    SAML 2.0 compliant external identity provider. Sent as\n    `Authorization: Bearer <token>`.\n  source: https://documentation.onestream.com/1375907/Content/IDM/OneStream%20IdentityServer.html\n- name: OAuth2ClientCredentials\n  type: oauth2\n  description: >-\n    OAuth 2.0 client_credentials grant for self-hosted environments federating\n    to a supported external provider (Microsoft Entra ID / Azure AD, Okta,\n    PingFederate). Requires Client ID, Client Secret, and the provider Token\n    URL; the returned access token is used as a bearer token on API calls.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: provider-specific (Azure AD / Okta / PingFederate token endpoint)\n    scopes: {}\n  source:\
  \ https://documentation.onestream.com/docs/Content/REST%20API/Configure%20OneStream%20API%20for%20External.html\nexternal_identity_providers:\n- Microsoft Entra ID (Azure Active Directory)\n- Okta\n- PingFederate\nidentity_protocols:\n- OIDC\n- SAML 2.0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onestream/refs/heads/main/authentication/onestream-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Software
- Finance
- Corporate Performance Management
- Financial Planning and Analysis
- Financial Close
- Consolidation
- Enterprise
- API
---
