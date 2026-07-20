---
api_key_in:
- header
api_specs:
- filename: just-eat-uk-openapi-original.json
  format: json
  label: Just Eat UK API
  slug: just-eat-uk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/just-eat/refs/heads/main/openapi/just-eat-uk-openapi-original.json
auth_types:
- apiKey
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Just Eat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Just Eat secures its APIs with apiKey, http, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Just Eat
provider_slug: just-eat
scheme_count: 4
schemes:
- bearerFormat: JWT
  description: Bearer token authentication using a JSON Web Token (JWT).
  name: Bearer
  scheme: bearer
  sources:
  - openapi/just-eat-uk-openapi-original.json
  type: http
- description: APIs for delivery partners require an API key that will have been issued to you.
  in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/just-eat-uk-openapi-original.json
  type: apiKey
- description: A few services allow the use of basic authentication when a partner doesn't support OAuth based authentication.
  name: basic_auth
  scheme: basic
  sources:
  - openapi/just-eat-uk-openapi-original.json
  type: http
- description: ADFS authentication provider for internal Just Eat tools.
  name: justeat_adfs
  openIdConnectUrl: https://adfs.just-eat.com/adfs/.well-known/openid-configuration
  sources:
  - openapi/just-eat-uk-openapi-original.json
  type: openIdConnect
slug: just-eat-authentication
source_filename: just-eat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/just-eat-uk-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - openIdConnect\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication using a JSON Web Token (JWT).\n  sources:\n  - openapi/just-eat-uk-openapi-original.json\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: APIs for delivery partners require an API key that will have been issued to you.\n  sources:\n  - openapi/just-eat-uk-openapi-original.json\n- name: basic_auth\n  type: http\n  scheme: basic\n  description: A few services allow the use of basic authentication when a partner doesn't support\n    OAuth based authentication.\n  sources:\n  - openapi/just-eat-uk-openapi-original.json\n- name: justeat_adfs\n  type: openIdConnect\n  openIdConnectUrl: https://adfs.just-eat.com/adfs/.well-known/openid-configuration\n\
  \  description: ADFS authentication provider for internal Just Eat tools.\n  sources:\n  - openapi/just-eat-uk-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/just-eat/refs/heads/main/authentication/just-eat-authentication.yml
summary_line: apiKey/http/openIdConnect · 4 schemes
tags:
- Food Delivery
- Restaurants
- Marketplace
- Logistics
- Orders
- Delivery
- Point of Sale
- E-commerce
---
