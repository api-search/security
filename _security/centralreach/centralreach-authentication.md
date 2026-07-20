---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: 'The CentralReach Enhanced API requires two credentials on every request: an organization-scoped API key sent in the x-api-key header, and an OAuth 2.0 Bearer access token obtained via the client-credentials grant against the CentralReach identity provider. Credentials (client_id, client_secret, and the CR API key) are issued by the CentralReach Implementation Team; the API is not self-serve. Access tokens are RS256 JWTs with a one-hour lifetime carrying iss, exp, sub, and orgid claims.'
kind: authentication
layout: security
method: searched
name: Centralreach Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CentralReach secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CentralReach
provider_slug: centralreach
scheme_count: 2
schemes:
- flow: clientCredentials
  name: clientCredentials
  scopes:
  - openid
  - cr
  - cr-api
  - offline_access
  sources:
  - https://login.centralreach.com/.well-known/openid-configuration
  tokenUrl: https://login.centralreach.com/connect/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- description: Organization-specific API key issued by the CentralReach Implementation Team.
  in: header
  name: apiKey
  parameter_name: x-api-key
  sources:
  - https://centralreach.com/resources/api/
  type: apiKey
slug: centralreach-authentication
source_filename: centralreach-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://login.centralreach.com/.well-known/openid-configuration\ndocs: https://centralreach.com/resources/api/\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  api_key_name: x-api-key\n  oauth2_flows: [clientCredentials]\n  identity_provider: https://login.centralreach.com\n  token_signing_alg: RS256\n  access_token_ttl_seconds: 3600\ndescription: >-\n  The CentralReach Enhanced API requires two credentials on every request: an\n  organization-scoped API key sent in the x-api-key header, and an OAuth 2.0\n  Bearer access token obtained via the client-credentials grant against the\n  CentralReach identity provider. Credentials (client_id, client_secret, and the\n  CR API key) are issued by the CentralReach Implementation Team; the API is not\n  self-serve. Access tokens are RS256 JWTs with a one-hour lifetime carrying iss,\n  exp, sub, and orgid claims.\nschemes:\n- name: clientCredentials\n  type: oauth2\n  flow:\
  \ clientCredentials\n  tokenUrl: https://login.centralreach.com/connect/token\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  scopes: [openid, cr, cr-api, offline_access]\n  sources: [https://login.centralreach.com/.well-known/openid-configuration]\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: Organization-specific API key issued by the CentralReach Implementation Team.\n  sources: [https://centralreach.com/resources/api/]\noidc:\n  issuer: https://login.centralreach.com\n  authorization_endpoint: https://login.centralreach.com/connect/authorize\n  token_endpoint: https://login.centralreach.com/connect/token\n  userinfo_endpoint: https://login.centralreach.com/connect/userinfo\n  jwks_uri: https://login.centralreach.com/.well-known/openid-configuration/jwks\n  introspection_endpoint: https://login.centralreach.com/connect/introspect\n  revocation_endpoint: https://login.centralreach.com/connect/revocation\n  grant_types_supported:\
  \ [authorization_code, client_credentials, refresh_token, implicit, password, 'urn:ietf:params:oauth:grant-type:device_code', 'urn:openid:params:grant-type:ciba']\n  code_challenge_methods_supported: [plain, S256]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centralreach/refs/heads/main/authentication/centralreach-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Healthcare
- ABA Therapy
- Autism
- IDD
- EMR
- Practice Management
- Behavioral Health
- Special Education
- Billing
- OAuth
---
