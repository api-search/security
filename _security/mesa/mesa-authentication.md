---
api_key_in:
- body
api_specs:
- filename: mesa-partner-api-openapi.yml
  format: yaml
  label: Mesa Partner API
  slug: mesa-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesa/refs/heads/main/openapi/mesa-partner-api-openapi.yml
auth_types:
- apiKey
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Mesa Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Mesa secures its APIs with apiKey, http, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Mesa
provider_slug: mesa
scheme_count: 3
schemes:
- description: clientId + clientSecret pair issued in the Mesa partner portal (partners.joinmesa.com). Sent in the JSON body of POST /token and POST /partners/{partnerId}/auth. Must stay server-side.
  in: body
  name: apiKeyCredentials
  sources:
  - openapi/mesa-partner-api-openapi.yml
  - https://docs.joinmesa.com/set-up/api-keys
  type: apiKey
- bearerFormat: JWT
  description: Short-lived JWT returned by the token endpoints; used on subsequent Partner API calls.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mesa-partner-api-openapi.yml
  type: http
- description: Optional end-user authentication via the partner's OpenID Provider (Okta, Azure AD, Google) using the Authorization Code flow with scopes openid, email, profile. The partner shares Issuer URL, Client ID, and Client Secret with Mesa; contact support@joinmesa.com to enable.
  name: oidc
  scopes:
  - openid
  - email
  - profile
  sources:
  - https://docs.joinmesa.com/embedded-ui/user-flows
  type: openIdConnect
slug: mesa-authentication
source_filename: mesa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.joinmesa.com/set-up/api-keys\ndocs: https://docs.joinmesa.com/embedded-ui/auth-flow\nsummary:\n  types: [apiKey, http, openIdConnect]\n  api_key_in: [body]\n  oauth2_flows: [authorizationCode]\n  model: >-\n    Server-side API keys (clientId + clientSecret) are exchanged for a short-lived JWT session token\n    scoped to a single end user (vendorId + userId). The JWT is used as a Bearer token on Partner API\n    calls and passed to the MesaClient embed handshake. End users authenticate either with Mesa native\n    sign-up/sign-in or via the partner's OIDC provider.\nschemes:\n- name: apiKeyCredentials\n  type: apiKey\n  in: body\n  description: >-\n    clientId + clientSecret pair issued in the Mesa partner portal (partners.joinmesa.com). Sent in\n    the JSON body of POST /token and POST /partners/{partnerId}/auth. Must stay server-side.\n  sources: [openapi/mesa-partner-api-openapi.yml, https://docs.joinmesa.com/set-up/api-keys]\n\
  - name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Short-lived JWT returned by the token endpoints; used on subsequent Partner API calls.\n  sources: [openapi/mesa-partner-api-openapi.yml]\n- name: oidc\n  type: openIdConnect\n  description: >-\n    Optional end-user authentication via the partner's OpenID Provider (Okta, Azure AD, Google) using\n    the Authorization Code flow with scopes openid, email, profile. The partner shares Issuer URL,\n    Client ID, and Client Secret with Mesa; contact support@joinmesa.com to enable.\n  scopes: [openid, email, profile]\n  sources: [https://docs.joinmesa.com/embedded-ui/user-flows]\njwt_payload:\n  origin: Allowed iframe origin; scopes the token to the partner domain.\n  partnerId: Mesa-assigned partner identifier.\n  programCode: Controls which payment programs appear in onboarding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mesa/refs/heads/main/authentication/mesa-authentication.yml
summary_line: apiKey/http/openIdConnect · 3 schemes
tags:
- Company
- Fintech
- Payments
- Invoice Financing
- Embedded Finance
- Early Payment
- ACH
- Supplier Payments
- B2B
---
