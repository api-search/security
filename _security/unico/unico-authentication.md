---
api_key_in: []
api_specs:
- filename: unico-api-integration.postman_collection.json
  format: json
  label: Unico IDCloud API
  slug: idcloud-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/unico/refs/heads/main/postman/unico-api-integration.postman_collection.json
- filename: unico-web-sdk-integration.postman_collection.json
  format: json
  label: Unico IDCloud Web & SDK API
  slug: idcloud-web-sdk
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/unico/refs/heads/main/postman/unico-web-sdk-integration.postman_collection.json
- filename: unico-oauth2.postman_collection.json
  format: json
  label: Unico Identity OAuth2
  slug: identity-oauth2
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/unico/refs/heads/main/postman/unico-oauth2.postman_collection.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Unico Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unico declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Unico
provider_slug: unico
scheme_count: 0
schemes: []
slug: unico-authentication
source_filename: unico-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://developer.unico.io/developers/api-reference/authentication\ndocs: https://developer.unico.io/developers/api-reference/authentication\nnote: >-\n  Unico publishes no OpenAPI, so this profile is read from the published Authentication and\n  Environments reference pages plus the live OpenID Connect discovery document served at\n  https://identity.acesso.io/.well-known/openid-configuration (HTTP 200, 2026-09-02).\n  identity.acesso.io is Unico's own token host: the Environments page names it as the\n  production OAuth2 endpoint for every IDCloud contract.\nsecurity_schemes:\n- name: unico_oauth2_jwt_bearer\n  type: oauth2\n  flow: urn:ietf:params:oauth:grant-type:jwt-bearer\n  rfc: RFC 7523 (JWT Profile for OAuth 2.0 Client Authentication and Authorization Grants)\n  token_endpoint_production: https://identity.acesso.io/oauth2/token\n  token_endpoint_sandbox: https://identityhomolog.acesso.io/oauth2/token\n  authorization_endpoint:\
  \ https://identity.acesso.io/oauth2/authorize\n  introspection_endpoint: https://identity.acesso.io/api/oauth2/tokeninfo\n  jwks_uri: https://identity.acesso.io/.well-known/jwks.json\n  request_content_type: application/x-www-form-urlencoded\n  assertion_parameter: assertion\n  signing_algorithm: RS256\n  assertion_claims:\n  - claim: iss\n    value: <account_name>@<tenant_id>.iam.acesso.io\n  - claim: aud\n    value: environment identity URL (https://identity.acesso.io or https://identityhomolog.acesso.io)\n  - claim: scope\n    value: '*'\n  - claim: iat\n    value: unix timestamp at issue\n  - claim: exp\n    value: maximum iat + 3600\n  token_ttl_seconds: 3600\n  renewal_guidance: >-\n    Reuse the access token for its full 1-hour TTL; refresh proactively when ~10 minutes\n    remain. The rate-limits page explicitly calls out per-request token minting as a way to\n    exhaust the tenant budget.\n- name: unico_bearer\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  header: 'Authorization:\
  \ Bearer <access_token>'\n  applies_to: all IDCloud contracts (Web & SDK, API)\n- name: unico_apikey\n  type: apiKey\n  in: header\n  header_name: APIKEY\n  applies_to: the API (TCA / Check.Integration) contract only\n  note: >-\n    The APIKEY is not a second credential so much as a capability selector — the provisioned\n    key decides which product (Onboarding, Transactional, Cardholder Verification) and which\n    capability recipe (flow) the tenant's process executes. Adding a capability requires the\n    key to be reissued.\ndiscovery:\n  openid_configuration: https://identity.acesso.io/.well-known/openid-configuration\n  http_status: 200\n  issuer: https://identity.acesso.io\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types_supported:\n  - code\n  subject_types_supported:\n  - public\n  id_token_signing_alg_values_supported:\n  - RS256\n  code_challenge_methods_supported:\n\
  \  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  - urn:ietf:params:oauth:client-assertion-type:jwt-bearer\ncredential_separation:\n  environments_share_no_credentials: true\n  note: >-\n    Sandbox and production use different Client ID, private key and API key. Unico's own docs\n    name credential mixing as the most common cause of 401.\ncommon_failures:\n- symptom: HTTP 401\n  causes:\n  - incorrect or mismatched RSA private key\n  - aud claim does not match the environment identity URL\n  - exp claim already past, or beyond iat + 3600\n  - signing algorithm other than RS256\n  - sandbox credentials sent to production (or the reverse)\n  - APIKEY header missing on the API contract\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unico/refs/heads/main/authentication/unico-authentication.yml
summary_line: 0 schemes
tags:
- Identity Verification
- Biometrics
- Facial Recognition
- Liveness Detection
- KYC
- Fraud Prevention
- Onboarding
- Authentication
- AML
- Age Verification
- Document Verification
- Identity
- Brazil
- Latin America
---
