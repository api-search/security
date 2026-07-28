---
api_key_in:
- header
- query
api_specs:
- filename: ercot-public-data-api-openapi.json
  format: json
  label: ERCOT Public Data API
  slug: ercot-public-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ercot/refs/heads/main/openapi/ercot-public-data-api-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: 'Every ERCOT Public Data API call carries TWO credentials, not one: an Azure API Management subscription key AND an Azure AD B2C ID token. The OpenAPI declares only the subscription-key half (apiKeyHeader / apiKeyQuery); the bearer half is documented only in the developer portal, so this profile is upgraded from the spec-derived baseline with the documented token flow. Registration is free and self-serve at the ERCOT API Explorer (email verification, then subscribe to a product to mint a subscription key). The market-participant SOAP estate (EWS, MarkeTrak, Retail API) uses a completely different model — ERCOT-issued digital certificates plus WS-Security — and is not reachable with these credentials.'
kind: authentication
layout: security
method: searched
name: Ercot Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: ERCOT secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: ERCOT
provider_slug: ercot
scheme_count: 4
schemes:
- description: Azure API Management subscription key, minted per product subscription in the API Explorer profile page.
  in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  required: true
  sources:
  - openapi/ercot-public-data-api-openapi.json
  - https://developer.ercot.com/applications/pubapi/user-guide/using-api/
  type: apiKey
- description: Query-string alternative to the Ocp-Apim-Subscription-Key header.
  in: query
  name: apiKeyQuery
  parameter: subscription-key
  required: false
  sources:
  - openapi/ercot-public-data-api-openapi.json
  type: apiKey
- bearerFormat: JWT
  description: 'Azure AD B2C ID token passed as `Authorization: Bearer <id_token>`. Not declared in the OpenAPI but mandatory — calls without it are rejected. Tokens are valid for one hour and cannot be refreshed; a new POST to the token endpoint mints another.'
  name: b2cIdToken
  required: true
  scheme: bearer
  sources:
  - https://developer.ercot.com/applications/pubapi/user-guide/registration-and-authentication/
  type: http
- authorization_url: https://ercotb2c.b2clogin.com/ercotb2c.onmicrosoft.com/b2c_1_pubapi-ropc-flow/oauth2/v2.0/authorize
  client_id: fec253ea-0d06-4272-a5e6-b478baeecd70
  description: Azure AD B2C Resource Owner Password Credentials (ROPC) user flow. The developer's portal username and password are POSTed directly to the token endpoint; the response carries access_token, refresh_token and the id_token the API actually consumes. ROPC is a legacy OAuth 2.0 grant — credentials are handled by the client, so they must be stored securely.
  flow: password
  grant_type: password
  issuer: https://ercotb2c.b2clogin.com/6df17afa-1b36-499a-83f7-56779ad0b9a6/v2.0/
  jwks_uri: https://ercotb2c.b2clogin.com/ercotb2c.onmicrosoft.com/b2c_1_pubapi-ropc-flow/discovery/v2.0/keys
  name: ercotB2C
  response_type: id_token
  scope: openid+fec253ea-0d06-4272-a5e6-b478baeecd70+offline_access
  sources:
  - https://developer.ercot.com/applications/pubapi/user-guide/registration-and-authentication/
  - well-known/ercot-openid-configuration.json
  token_lifetime_seconds: 3600
  token_url: https://ercotb2c.b2clogin.com/ercotb2c.onmicrosoft.com/B2C_1_PUBAPI-ROPC-FLOW/oauth2/v2.0/token
  type: oauth2
slug: ercot-authentication
source_filename: ercot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/ercot-public-data-api-openapi.json\ndocs: https://developer.ercot.com/applications/pubapi/user-guide/registration-and-authentication/\ndescription: >-\n  Every ERCOT Public Data API call carries TWO credentials, not one: an Azure API Management\n  subscription key AND an Azure AD B2C ID token. The OpenAPI declares only the subscription-key\n  half (apiKeyHeader / apiKeyQuery); the bearer half is documented only in the developer portal,\n  so this profile is upgraded from the spec-derived baseline with the documented token flow.\n  Registration is free and self-serve at the ERCOT API Explorer (email verification, then\n  subscribe to a product to mint a subscription key). The market-participant SOAP estate\n  (EWS, MarkeTrak, Retail API) uses a completely different model — ERCOT-issued digital\n  certificates plus WS-Security — and is not reachable with these credentials.\nsummary:\n  types:\n  - apiKey\n  - http\n \
  \ - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - password\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  required: true\n  description: Azure API Management subscription key, minted per product subscription in the API Explorer profile page.\n  sources:\n  - openapi/ercot-public-data-api-openapi.json\n  - https://developer.ercot.com/applications/pubapi/user-guide/using-api/\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  required: false\n  description: Query-string alternative to the Ocp-Apim-Subscription-Key header.\n  sources:\n  - openapi/ercot-public-data-api-openapi.json\n- name: b2cIdToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  required: true\n  description: >-\n    Azure AD B2C ID token passed as `Authorization: Bearer <id_token>`. Not declared in the\n    OpenAPI but mandatory — calls without it are rejected. Tokens are valid for one hour and\n   \
  \ cannot be refreshed; a new POST to the token endpoint mints another.\n  sources:\n  - https://developer.ercot.com/applications/pubapi/user-guide/registration-and-authentication/\n- name: ercotB2C\n  type: oauth2\n  flow: password\n  grant_type: password\n  token_url: https://ercotb2c.b2clogin.com/ercotb2c.onmicrosoft.com/B2C_1_PUBAPI-ROPC-FLOW/oauth2/v2.0/token\n  authorization_url: https://ercotb2c.b2clogin.com/ercotb2c.onmicrosoft.com/b2c_1_pubapi-ropc-flow/oauth2/v2.0/authorize\n  jwks_uri: https://ercotb2c.b2clogin.com/ercotb2c.onmicrosoft.com/b2c_1_pubapi-ropc-flow/discovery/v2.0/keys\n  issuer: https://ercotb2c.b2clogin.com/6df17afa-1b36-499a-83f7-56779ad0b9a6/v2.0/\n  client_id: fec253ea-0d06-4272-a5e6-b478baeecd70\n  scope: openid+fec253ea-0d06-4272-a5e6-b478baeecd70+offline_access\n  response_type: id_token\n  token_lifetime_seconds: 3600\n  description: >-\n    Azure AD B2C Resource Owner Password Credentials (ROPC) user flow. The developer's portal\n    username and password\
  \ are POSTed directly to the token endpoint; the response carries\n    access_token, refresh_token and the id_token the API actually consumes. ROPC is a legacy\n    OAuth 2.0 grant — credentials are handled by the client, so they must be stored securely.\n  sources:\n  - https://developer.ercot.com/applications/pubapi/user-guide/registration-and-authentication/\n  - well-known/ercot-openid-configuration.json\nregistration:\n  url: https://apiexplorer.ercot.com/\n  self_serve: true\n  cost: free\n  steps:\n  - Sign up on the ERCOT API Explorer with an email address and verification code.\n  - Subscribe to a product on the Products page to mint a subscription key.\n  - Copy the Primary key from the profile page (once — it is reusable).\n  - POST username/password to the B2C token endpoint for an ID token (repeat hourly).\nother_estates:\n- api: ERCOT Web Services (EWS)\n  model: ERCOT-issued digital certificate + WS-Security (WSS 2004/01) over SOAP\n  audience: registered ERCOT Market Participants\
  \ only\n- api: ERCOT MarkeTrak API\n  model: ERCOT digital certificate; application must pass ERCOT certification before production access\n  audience: registered ERCOT Market Participants only\n- api: ERCOT Retail API\n  model: ERCOT digital certificate over SOAP (TX SET transactions)\n  audience: certified Market Participants only\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ercot/refs/heads/main/authentication/ercot-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Energy
- United States
- Electricity
- Energy Markets
- Grid
- System Operator
- Texas
- Renewables
- Demand Response
- Open Data
---
