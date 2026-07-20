---
api_key_in:
- header
- cookie
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Centrify Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- password
overview: Centrify secures its APIs with oauth2, http, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, and password flow(s).
provider_name: Centrify
provider_slug: centrify
scheme_count: 4
schemes:
- description: OAuth2 confidential-client flows against the tenant OAuth2 authorization server; used for programmatic / service access to the Centrify REST API.
  flows:
  - flow: clientCredentials
  - flow: authorizationCode
  - flow: password
  name: OAuth2
  type: oauth2
- description: API access tokens (bearer) issued after authentication, sent on subsequent REST calls.
  name: BearerToken
  scheme: bearer
  type: http
- description: Authentication cookie established by the interactive/adaptive authentication flow (MFA-aware) for portal-scoped calls.
  in: cookie
  name: SessionCookie
  type: apiKey
- description: SAML assertions accepted for federated/SSO scenarios into the Identity Platform.
  name: SAML
  type: other
slug: centrify-authentication
source_filename: centrify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.delinea.com/docs/getting-access-to-the-api\ndocs: https://developer.delinea.com/docs/using-apis\nnote: >-\n  Derived from the Centrify Identity Services / Cloud Suite (PAS) developer\n  documentation (served at developer.delinea.com after the Delinea rebrand).\n  No machine-readable OpenAPI is captured in this repo, so this profile is\n  documented from the published auth guides rather than derived from a spec.\nsummary:\n  types: [oauth2, http, apiKey]\n  api_key_in: [header, cookie]\n  oauth2_flows: [clientCredentials, authorizationCode, password]\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n  - flow: authorizationCode\n  - flow: password\n  description: >-\n    OAuth2 confidential-client flows against the tenant OAuth2 authorization\n    server; used for programmatic / service access to the Centrify REST API.\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description:\
  \ >-\n    API access tokens (bearer) issued after authentication, sent on subsequent\n    REST calls.\n- name: SessionCookie\n  type: apiKey\n  in: cookie\n  description: >-\n    Authentication cookie established by the interactive/adaptive\n    authentication flow (MFA-aware) for portal-scoped calls.\n- name: SAML\n  type: other\n  description: >-\n    SAML assertions accepted for federated/SSO scenarios into the Identity\n    Platform.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrify/refs/heads/main/authentication/centrify-authentication.yml
summary_line: oauth2/http/apiKey · 4 schemes
tags:
- Company
- Identity
- Privileged Access Management
- Access Management
- Authentication
- Single Sign-On
- Multi-Factor Authentication
- Security
- Zero Trust
- IAM
---
