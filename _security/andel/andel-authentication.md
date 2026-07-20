---
api_key_in: []
api_specs:
- filename: andel-data-exchange-openapi.yaml
  format: yaml
  label: Data Exchange API
  slug: data-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/andel/refs/heads/main/openapi/andel-data-exchange-openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Andel Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Andel secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Andel
provider_slug: andel
scheme_count: 2
schemes:
- description: Production machine-to-machine flow. Tokens issued by Descope.
  grant: clientCredentials
  name: andelDescopeClientCredentials
  scheme: bearer
  scopes:
  - purchases:read
  sources:
  - openapi/andel-data-exchange-openapi.yaml
  token_url: https://api.descope.com/oauth2/v1/apps/token
  type: http
- description: Developer-exploration flow with PKCE. Used by Postman Guided Auth.
  grant: authorizationCode
  name: andelDescopeAuthCode
  scheme: bearer
  sources:
  - openapi/andel-data-exchange-openapi.yaml
  type: http
slug: andel-authentication
source_filename: andel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/andel-data-exchange-openapi.yaml\ndocs: https://build.andel.org/dataexchange/overview/overview\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  token_issuer: Descope\n  token_url: https://api.descope.com/oauth2/v1/apps/token\n  scopes:\n  - purchases:read\n  notes: >-\n    Production is an OAuth 2.0 client-credentials (machine-to-machine) flow with\n    tokens issued by Descope and presented as HTTP bearer tokens. Access tokens\n    carry a `plans` claim used for per-plan authorization enforcement. A\n    developer-exploration authorization-code + PKCE flow (Postman Guided Auth)\n    is also supported. The OpenAPI models both as `http`/`bearer` schemes; the\n    OAuth grant detail is documented in the Data Exchange overview.\nschemes:\n- name: andelDescopeClientCredentials\n  type: http\n  scheme: bearer\n  grant: clientCredentials\n  token_url: https://api.descope.com/oauth2/v1/apps/token\n\
  \  scopes:\n  - purchases:read\n  description: Production machine-to-machine flow. Tokens issued by Descope.\n  sources:\n  - openapi/andel-data-exchange-openapi.yaml\n- name: andelDescopeAuthCode\n  type: http\n  scheme: bearer\n  grant: authorizationCode\n  description: Developer-exploration flow with PKCE. Used by Postman Guided Auth.\n  sources:\n  - openapi/andel-data-exchange-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andel/refs/heads/main/authentication/andel-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Healthcare
- Pharmacy
- Pharmacy Benefits
- Drug Pricing
- Specialty Medications
- Data Exchange
- Webhooks
---
