---
api_key_in:
- header
api_specs:
- filename: revinate-hotel-sets-api-openapi.yml
  format: yaml
  label: Revinate Hotel Sets API
  slug: revinate-hotel-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revinate/refs/heads/main/openapi/revinate-hotel-sets-api-openapi.yml
- filename: revinate-hotels-api-openapi.yml
  format: yaml
  label: Revinate Hotels API
  slug: revinate-hotels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revinate/refs/heads/main/openapi/revinate-hotels-api-openapi.yml
- filename: revinate-languages-api-openapi.yml
  format: yaml
  label: Revinate Languages API
  slug: revinate-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revinate/refs/heads/main/openapi/revinate-languages-api-openapi.yml
- filename: revinate-review-sites-api-openapi.yml
  format: yaml
  label: Revinate Review Sites API
  slug: revinate-review-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revinate/refs/heads/main/openapi/revinate-review-sites-api-openapi.yml
- filename: revinate-reviews-api-openapi.yml
  format: yaml
  label: Revinate Reviews API
  slug: revinate-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revinate/refs/heads/main/openapi/revinate-reviews-api-openapi.yml
- filename: revinate-widget-reviews-api-openapi.yml
  format: yaml
  label: Revinate Widget Reviews API
  slug: revinate-widget-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revinate/refs/heads/main/openapi/revinate-widget-reviews-api-openapi.yml
auth_types:
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Revinate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revinate secures its APIs with apiKey and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Revinate
provider_slug: revinate
scheme_count: 4
schemes:
- description: Username with access to the requested resources and to the API key used.
  in: header
  name: porterUsername
  parameter: X-Revinate-Porter-Username
  sources:
  - openapi/revinate-porter-openapi.yml
  - https://porter.revinate.com/documentation
  type: apiKey
- description: Epoch-seconds timestamp; must be within 5 minutes (before or after) of the request.
  in: header
  name: porterTimestamp
  parameter: X-Revinate-Porter-Timestamp
  sources:
  - openapi/revinate-porter-openapi.yml
  - https://porter.revinate.com/documentation
  type: apiKey
- description: API key issued by Revinate (contact your sales rep or account manager).
  in: header
  name: porterKey
  parameter: X-Revinate-Porter-Key
  sources:
  - openapi/revinate-porter-openapi.yml
  - https://porter.revinate.com/documentation
  type: apiKey
- description: HMAC_SHA256(apiSecret, username + timestamp), hex-encoded.
  in: header
  name: porterEncoded
  parameter: X-Revinate-Porter-Encoded
  sources:
  - openapi/revinate-porter-openapi.yml
  - https://porter.revinate.com/documentation
  type: apiKey
slug: revinate-authentication
source_filename: revinate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://porter.revinate.com/documentation\ndocs: https://porter.revinate.com/documentation#authentication-and-access-control\nsummary:\n  types:\n  - apiKey\n  - openIdConnect\n  api_key_in:\n  - header\n  models: 2\nnote: >-\n  Revinate operates two separate and unrelated authentication models. The public Porter REST API\n  uses a bespoke four-header HMAC-SHA256 request-signing scheme with no OAuth and no scopes. The\n  Revinate web application (home.revinate.com) is fronted by an Auth0-backed OpenID Connect issuer\n  at auth.revinate.com. An integrator calling the Porter API uses only the first model.\nmodels:\n- id: porter-hmac\n  name: Porter API HMAC-SHA256 header signing\n  applies_to: https://porter.revinate.com\n  type: apiKey\n  transport: header\n  standard: false\n  description: >-\n    Every authenticated Porter resource requires four request headers. Three carry identity and the\n    fourth carries a keyed digest\
  \ proving possession of the API secret. The secret itself is never\n    transmitted. Credentials are not self-service — the documentation directs integrators to contact\n    their Revinate sales representative or account manager for an API key and secret with the\n    appropriate access permissions.\n  headers:\n  - name: X-Revinate-Porter-Username\n    required: true\n    description: A username that has access both to the resources requested and to the API key used.\n  - name: X-Revinate-Porter-Timestamp\n    required: true\n    description: >-\n      Epoch-seconds timestamp. Must be within 5 minutes before or after the moment the request is\n      sent, which bounds replay of a captured signature to a 10-minute window.\n  - name: X-Revinate-Porter-Key\n    required: true\n    description: The API key issued by Revinate.\n  - name: X-Revinate-Porter-Encoded\n    required: true\n    description: >-\n      HMAC_SHA256(apiSecret, username + timestamp), hex-encoded. The signed string is\
  \ the plain\n      concatenation of the username and the epoch-seconds timestamp; the API secret is the HMAC key.\n  signing:\n    algorithm: HMAC-SHA256\n    encoding: hexadecimal\n    signed_string: username + timestamp (string concatenation, no separator)\n    key: API secret issued by Revinate\n    replay_window_seconds: 300\n  credential_issuance: manual — via Revinate sales representative or account manager\n  self_service: false\n  observed_failure:\n    status: 401\n    body_shape: '{\"timestamp\":<epoch_ms>,\"status\":401,\"error\":\"Unauthorized\",\"message\":\"...\",\"path\":\"...\"}'\n    note: Observed live on 2026-08-26 against https://porter.revinate.com/ with no auth headers.\n  code_samples_published:\n  - Shell (openssl)\n  - Java (javax.crypto.Mac)\n  - Ruby (OpenSSL::HMAC)\n  - C# (System.Security.Cryptography.HMACSHA256)\n- id: revinate-oidc\n  name: Revinate application OpenID Connect\n  applies_to: https://home.revinate.com\n  type: openIdConnect\n  standard: true\n\
  \  openid_configuration: https://auth.revinate.com/.well-known/openid-configuration\n  issuer: https://auth.revinate.com/\n  authorization_endpoint: https://auth.revinate.com/authorize\n  token_endpoint: https://auth.revinate.com/oauth/token\n  userinfo_endpoint: https://auth.revinate.com/userinfo\n  jwks_uri: https://auth.revinate.com/.well-known/jwks.json\n  revocation_endpoint: https://auth.revinate.com/oauth/revoke\n  device_authorization_endpoint: https://auth.revinate.com/oauth/device/code\n  registration_endpoint: https://auth.revinate.com/oidc/register\n  mfa_challenge_endpoint: https://auth.revinate.com/mfa/challenge\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\n  id_token_signing_alg:\n  - RS256\n  - HS256\n  - PS256\n  provider: Auth0\n  description: >-\n    Full OIDC issuer securing the Revinate application UI. Supports authorization code with PKCE,\n    client credentials, refresh tokens, device code, and token exchange. Dynamic client registration\n    is advertised.\
  \ This surface does not grant access to the Porter API.\n  scopes: scopes/revinate-scopes.yml\nschemes:\n- name: porterUsername\n  type: apiKey\n  in: header\n  parameter: X-Revinate-Porter-Username\n  description: Username with access to the requested resources and to the API key used.\n  sources:\n  - openapi/revinate-porter-openapi.yml\n  - https://porter.revinate.com/documentation\n- name: porterTimestamp\n  type: apiKey\n  in: header\n  parameter: X-Revinate-Porter-Timestamp\n  description: Epoch-seconds timestamp; must be within 5 minutes (before or after) of the request.\n  sources:\n  - openapi/revinate-porter-openapi.yml\n  - https://porter.revinate.com/documentation\n- name: porterKey\n  type: apiKey\n  in: header\n  parameter: X-Revinate-Porter-Key\n  description: API key issued by Revinate (contact your sales rep or account manager).\n  sources:\n  - openapi/revinate-porter-openapi.yml\n  - https://porter.revinate.com/documentation\n- name: porterEncoded\n  type: apiKey\n \
  \ in: header\n  parameter: X-Revinate-Porter-Encoded\n  description: HMAC_SHA256(apiSecret, username + timestamp), hex-encoded.\n  sources:\n  - openapi/revinate-porter-openapi.yml\n  - https://porter.revinate.com/documentation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revinate/refs/heads/main/authentication/revinate-authentication.yml
summary_line: apiKey/openIdConnect · 4 schemes
tags:
- Hospitality
- Hotels
- Reviews
- Reputation Management
- Guest Data Platform
- CRM
- Sentiment Analysis
- Travel
- Marketing
- Customer Feedback
---
