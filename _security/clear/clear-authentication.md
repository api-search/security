---
api_key_in: []
api_specs:
- filename: clear-verification-openapi.json
  format: json
  label: CLEAR1 Verification Sessions API
  slug: clear1-verification-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear/refs/heads/main/openapi/clear-verification-openapi.json
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Clear Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CLEAR secures its APIs with http, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CLEAR
provider_slug: clear
scheme_count: 2
schemes:
- description: 'API key passed as a Bearer token: Authorization: Bearer <API_KEY>. Separate sandbox and production keys. HTTPS required.'
  name: Authorization_Bearer
  scheme: bearer
  sources:
  - openapi/clear-verification-openapi.json
  type: http
- authorizationUrl: https://verified.clearme.com/integrations/oauth2/auth
  description: OAuth 2.0 / OpenID Connect for end-user identity tokens, with PKCE (S256). Issuer https://verified.clearme.com/integrations.
  name: OAuth2_OIDC
  scheme: authorizationCode
  scopes:
  - openid
  - offline
  - offline_access
  sources:
  - https://docs.clearme.com/docs/oidc-identity-token
  - well-known/clear-openid-configuration.json
  tokenUrl: https://verified.clearme.com/integrations/oauth2/token
  type: oauth2
slug: clear-authentication
source_filename: clear-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/clear-verification-openapi.json\ndocs: https://docs.clearme.com/reference/api-keys\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: Authorization_Bearer\n  type: http\n  scheme: bearer\n  description: 'API key passed as a Bearer token: Authorization: Bearer <API_KEY>. Separate sandbox and production keys. HTTPS required.'\n  sources:\n  - openapi/clear-verification-openapi.json\n- name: OAuth2_OIDC\n  type: oauth2\n  scheme: authorizationCode\n  description: OAuth 2.0 / OpenID Connect for end-user identity tokens, with PKCE (S256). Issuer https://verified.clearme.com/integrations.\n  authorizationUrl: https://verified.clearme.com/integrations/oauth2/auth\n  tokenUrl: https://verified.clearme.com/integrations/oauth2/token\n  scopes:\n  - openid\n  - offline\n  - offline_access\n  sources:\n  - https://docs.clearme.com/docs/oidc-identity-token\n\
  \  - well-known/clear-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clear/refs/heads/main/authentication/clear-authentication.yml
summary_line: http/oauth2/openIdConnect · 2 schemes
tags:
- Company
- Identity
- Identity Verification
- Authentication
- KYC
- Biometrics
- OAuth
- OpenID Connect
- Healthcare
- Financial Services
---
