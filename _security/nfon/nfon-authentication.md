---
api_key_in: []
api_specs:
- filename: nfon-pbx-configuration-api-openapi.json
  format: json
  label: NFON PBX Configuration API
  slug: nfon-pbx-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/openapi/nfon-pbx-configuration-api-openapi.json
- filename: nfon-cti-api-openapi.yml
  format: yaml
  label: NFON CTI API
  slug: nfon-cti-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/openapi/nfon-cti-api-openapi.yml
- filename: nfon-call-history-api-openapi.yml
  format: yaml
  label: NFON Call History API
  slug: nfon-call-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/openapi/nfon-call-history-api-openapi.yml
- filename: nfon-service-portal-api.postman_collection.json
  format: json
  label: NFON Service Portal API (legacy)
  slug: nfon-service-portal-api-legacy
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/postman/nfon-service-portal-api.postman_collection.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nfon Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Nfon secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Nfon
provider_slug: nfon
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JSON Web Token bearer, applied to every operation across all three APIs.
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/nfon-call-history-api-openapi.yml
  - openapi/nfon-cti-api-openapi.yml
  - openapi/nfon-pbx-configuration-api-openapi.json
  type: http
slug: nfon-authentication
source_filename: nfon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nfon-call-history-api-openapi.yml, openapi/nfon-cti-api-openapi.yml, openapi/nfon-pbx-configuration-api-openapi.json\ndocs: https://www.nfon.com/en/integrations/api\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\nidentity_provider: https://sso.cloud-cfg.com/\nnotes: >-\n  All NFON APIs authenticate with an Authorization Bearer JWT. Three distinct\n  token-acquisition models are documented, one per API. Access is provisioned\n  by contacting integration@nfon.com. A User-Agent header of the form\n  \"<productname>/<productversion> (<K-Account>)\" is required on all requests.\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JSON Web Token bearer, applied to every operation across all three APIs.\n  sources:\n  - openapi/nfon-call-history-api-openapi.yml\n  - openapi/nfon-cti-api-openapi.yml\n  - openapi/nfon-pbx-configuration-api-openapi.json\n\
  token_acquisition:\n- api: NFON PBX Configuration API\n  model: oauth2-client-credentials\n  identity_provider: https://sso.cloud-cfg.com/\n  credentials: Client ID + Client Secret (request via integration@nfon.com)\n  notes: Machine-to-machine OAuth 2.0 client credentials flow; browser login via Login with NFON also supported.\n- api: NFON Call History API\n  model: oauth2-authorization-code-pkce\n  identity_provider: https://sso.cloud-cfg.com/\n  offering: Login with NFON (Early Access)\n  notes: Standard OAuth 2.0 Authorization Code flow with PKCE; partners receive their own OAuth client. Browser login via Cloudya (https://start.cloudya.com/).\n- api: NFON CTI API\n  model: custom-token-exchange\n  login_operation: createToken (POST /login)\n  refresh_operation: refreshAccessToken (PUT /login)\n  credentials: API Username + API Password\n  access_token_ttl_seconds: 300\n  jwks: /.well-known/jwks.json (publicKeyWellKnown)\n  notes: Username/password exchanged for a short-lived (5 minute)\
  \ access + refresh token pair; tokens are RS-signed JWTs verifiable via the published JWKS.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/authentication/nfon-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Company
- Telecom
- Cloud Telephony
- UCaaS
- CPaaS
- VoIP
- CTI
- Call History
- PBX
- Communications
- SIP
- Germany
---
