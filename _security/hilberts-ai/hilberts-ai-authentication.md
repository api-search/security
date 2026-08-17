---
api_key_in:
- header
api_specs:
- filename: hilberts-ai-program-api-openapi.yml
  format: yaml
  label: Hilbert's Program API
  slug: hilberts-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilberts-ai/refs/heads/main/openapi/hilberts-ai-program-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Hilberts Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
overview: Hilbert's AI secures its APIs with apiKey, http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and deviceCode flow(s).
provider_name: Hilbert's AI
provider_slug: hilberts-ai
scheme_count: 3
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hilberts-ai-program-api-openapi.yml
  type: http
- description: API key for server to server authentication
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/hilberts-ai-program-api-openapi.yml
  type: apiKey
- audience: https://app-api.hilberts.ai
  id_token_signing_alg:
  - HS256
  - RS256
  - PS256
  issuer: https://hilbert-app.us.auth0.com/
  jwks_uri: https://hilbert-app.us.auth0.com/.well-known/jwks.json
  name: auth0-oidc
  note: Issuer of the bearerAuth JWT declared in the OpenAPI. Not declared as a securityScheme in the spec; established by probe.
  openIdConnectUrl: https://hilbert-app.us.auth0.com/.well-known/openid-configuration
  pkce: true
  sources:
  - https://hilbert-app.us.auth0.com/.well-known/openid-configuration
  token_endpoint: https://hilbert-app.us.auth0.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: hilberts-ai-authentication
source_filename: hilberts-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/hilberts-ai-program-api-openapi.yml + https://hilbert-app.us.auth0.com/.well-known/openid-configuration\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - deviceCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/hilberts-ai-program-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for server to server authentication\n  sources:\n  - openapi/hilberts-ai-program-api-openapi.yml\n- name: auth0-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://hilbert-app.us.auth0.com/.well-known/openid-configuration\n  issuer: https://hilbert-app.us.auth0.com/\n  audience: https://app-api.hilberts.ai\n  token_endpoint: https://hilbert-app.us.auth0.com/oauth/token\n  jwks_uri: https://hilbert-app.us.auth0.com/.well-known/jwks.json\n\
  \  id_token_signing_alg:\n  - HS256\n  - RS256\n  - PS256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  pkce: true\n  sources:\n  - https://hilbert-app.us.auth0.com/.well-known/openid-configuration\n  note: Issuer of the bearerAuth JWT declared in the OpenAPI. Not declared as a securityScheme\n    in the spec; established by probe.\ndocs: null\nnote: The two schemes below are declared verbatim in the provider's own OpenAPI. The\n  bearer JWT is issued by Hilbert's Auth0 tenant hilbert-app.us.auth0.com (audience\n  https://app-api.hilberts.ai), confirmed from the app.hilberts.ai JavaScript bundle\n  and from the tenant's live OIDC discovery document. Hilbert publishes no authentication\n  guide, no key-issuance page and no developer portal, so how an x-api-key is obtained\n  is not documented anywhere public.\nscopes: scopes/hilberts-ai-scopes.yml\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://hilbert-app.us.auth0.com/.well-known/openid-configuration\n\
  \  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hilberts-ai/refs/heads/main/authentication/hilberts-ai-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Artificial Intelligence
- Growth
- Analytics
- Marketing
- Data Science
- Automation
- Agentic AI
- B2C
---
