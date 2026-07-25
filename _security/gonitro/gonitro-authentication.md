---
api_key_in: []
api_specs:
- filename: gonitro-authentication-api-openapi.yml
  format: yaml
  label: GoNitro Authentication API
  slug: gonitro-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gonitro/refs/heads/main/openapi/gonitro-authentication-api-openapi.yml
- filename: gonitro-conversions-api-openapi.yml
  format: yaml
  label: GoNitro Conversions API
  slug: gonitro-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gonitro/refs/heads/main/openapi/gonitro-conversions-api-openapi.yml
- filename: gonitro-extractions-api-openapi.yml
  format: yaml
  label: GoNitro Extractions API
  slug: gonitro-extractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gonitro/refs/heads/main/openapi/gonitro-extractions-api-openapi.yml
- filename: gonitro-generations-api-openapi.yml
  format: yaml
  label: GoNitro Generations API
  slug: gonitro-generations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gonitro/refs/heads/main/openapi/gonitro-generations-api-openapi.yml
- filename: gonitro-jobs-api-openapi.yml
  format: yaml
  label: GoNitro Jobs API
  slug: gonitro-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gonitro/refs/heads/main/openapi/gonitro-jobs-api-openapi.yml
- filename: gonitro-platform-api-openapi.yml
  format: yaml
  label: GoNitro Platform API
  slug: gonitro-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gonitro/refs/heads/main/openapi/gonitro-platform-api-openapi.yml
- filename: gonitro-sign-api-openapi.yml
  format: yaml
  label: GoNitro Sign API
  slug: gonitro-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gonitro/refs/heads/main/openapi/gonitro-sign-api-openapi.yml
- filename: gonitro-transformations-api-openapi.yml
  format: yaml
  label: GoNitro Transformations API
  slug: gonitro-transformations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gonitro/refs/heads/main/openapi/gonitro-transformations-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Gonitro Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: GoNitro secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: GoNitro
provider_slug: gonitro
scheme_count: 2
schemes:
- applied_globally: true
  bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gonitro-sign-openapi.json
  - openapi/gonitro-pdf-services-openapi.json
  type: http
- flow: clientCredentials
  name: OAuth2ClientCredentials
  note: Documented client-credentials flow. The OpenAPI declares the resulting bearer token as securityScheme `bearerAuth`; the token endpoint accepts clientID/clientSecret JSON (AuthTokenRequest) and returns an RFC 6749 OAuth2 token response. No OAuth scopes are defined.
  sources:
  - openapi/gonitro-sign-openapi.json
  tokenUrl: https://api.gonitro.dev/oauth/token
  type: oauth2
slug: gonitro-authentication
source_filename: gonitro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/gonitro-sign-openapi.json, openapi/gonitro-pdf-services-openapi.json\ndocs: https://developers.gonitro.com/docs/authentication/credentials\nsummary:\n  types:\n  - http\n  - oauth2\n  model: >-\n    Machine-to-machine OAuth 2.0 Client Credentials grant (RFC 6749). Create an\n    API application in the Nitro Admin Portal to obtain a Client ID and Client\n    Secret, exchange them at the token endpoint for a short-lived JWT access\n    token, then send it as an HTTP Bearer token on every API request.\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  token_endpoint: https://api.gonitro.dev/oauth/token\n  token_operation: getTokenRfc6749\n  token_format: JWT\n  token_response_fields:\n  - access_token\n  - token_type\n  - expires_in\n  credential_rotation: https://developers.gonitro.com/docs/authentication/credential-rotation\n  scopes: none\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat:\
  \ JWT\n  applied_globally: true\n  sources:\n  - openapi/gonitro-sign-openapi.json\n  - openapi/gonitro-pdf-services-openapi.json\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://api.gonitro.dev/oauth/token\n  note: >-\n    Documented client-credentials flow. The OpenAPI declares the resulting\n    bearer token as securityScheme `bearerAuth`; the token endpoint accepts\n    clientID/clientSecret JSON (AuthTokenRequest) and returns an RFC 6749\n    OAuth2 token response. No OAuth scopes are defined.\n  sources:\n  - openapi/gonitro-sign-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gonitro/refs/heads/main/authentication/gonitro-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Documents
- PDF
- eSignature
- Electronic Signatures
- Document Automation
- Document Conversion
- Data Extraction
- Redaction
- OCR
- Productivity
- Compliance
---
