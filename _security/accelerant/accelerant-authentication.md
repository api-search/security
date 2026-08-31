---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Accelerant Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Accelerant secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Accelerant
provider_slug: accelerant
scheme_count: 1
schemes:
- authorization_endpoint: https://app.accelerant.ai/api/auth/oidc/authorize
  claims_supported:
  - sub
  - name
  - email
  - profile
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://app.accelerant.ai
  jwks_uri: https://app.accelerant.ai/.well-known/jwks.json
  name: AccelerantPlatformOIDC
  openIdConnectUrl: https://app.accelerant.ai/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - profile
  - name
  - email
  sources:
  - well-known/accelerant-openid-configuration.json
  - well-known/accelerant-jwks.json
  subject_types_supported:
  - public
  token_endpoint: https://app.accelerant.ai/api/auth/oidc/token
  type: openIdConnect
  userinfo_endpoint: https://app.accelerant.ai/api/auth/oidc/userinfo
slug: accelerant-authentication
source_filename: accelerant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://app.accelerant.ai/.well-known/openid-configuration\ndocs: https://docs.accelerant.ai/\nnote: 'Derived from the anonymous OpenID Connect discovery document published by the\n  Accelerant Risk Exchange platform. No OpenAPI securitySchemes were available — the\n  API host (api.accelerant.ai) and the developer documentation (docs.accelerant.ai)\n  are both gated, so the OIDC discovery document is the only machine-readable auth\n  contract Accelerant publishes anonymously.'\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: AccelerantPlatformOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://app.accelerant.ai/.well-known/openid-configuration\n  issuer: https://app.accelerant.ai\n  authorization_endpoint: https://app.accelerant.ai/api/auth/oidc/authorize\n  token_endpoint: https://app.accelerant.ai/api/auth/oidc/token\n  userinfo_endpoint: https://app.accelerant.ai/api/auth/oidc/userinfo\n\
  \  jwks_uri: https://app.accelerant.ai/.well-known/jwks.json\n  response_types_supported:\n  - code\n  subject_types_supported:\n  - public\n  id_token_signing_alg_values_supported:\n  - RS256\n  scopes_supported:\n  - openid\n  - profile\n  - name\n  - email\n  claims_supported:\n  - sub\n  - name\n  - email\n  - profile\n  sources:\n  - well-known/accelerant-openid-configuration.json\n  - well-known/accelerant-jwks.json\ngaps:\n- 'No RFC 8414 OAuth 2.0 Authorization Server Metadata document is served anonymously\n  (/.well-known/oauth-authorization-server returns 401).'\n- 'No RFC 9728 OAuth 2.0 Protected Resource Metadata document is served anonymously.'\n- 'The API host api.accelerant.ai publishes no authentication metadata; its auth model\n  for Member system-to-system integration is documented only behind the gated developer\n  portal.'\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://app.accelerant.ai/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelerant/refs/heads/main/authentication/accelerant-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Insurance
- InsurTech
- Specialty Insurance
- Underwriting
- Risk Management
- Reinsurance
- Marketplace
- Risk Scoring
- Financial-Services
- Artificial Intelligence
---
