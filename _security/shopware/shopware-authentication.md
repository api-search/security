---
api_key_in:
- header
api_specs:
- filename: adminapi.json
  format: json
  label: Shopware Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/shopware/admin-api-reference/main/adminapi.json
- filename: storeapi.json
  format: json
  label: Shopware Store API
  slug: store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/shopware/store-api-reference/main/storeapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Shopware Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Shopware secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Shopware
provider_slug: shopware
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: /api/oauth/token
  - flow: password
    scopes: 1
    tokenUrl: /api/oauth/token
  name: oAuth2
  sources:
  - openapi/shopware-admin-api-openapi.yml
  type: oauth2
- description: Sales channel access key
  in: header
  name: swAccessKey
  parameter: sw-access-key
  sources:
  - openapi/shopware-store-api-openapi.yml
  type: apiKey
slug: shopware-authentication
source_filename: shopware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shopware-admin-api-openapi.yml, openapi/shopware-store-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  - password\nschemes:\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/oauth/token\n    scopes: 1\n  - flow: password\n    tokenUrl: /api/oauth/token\n    scopes: 1\n  sources:\n  - openapi/shopware-admin-api-openapi.yml\n- name: swAccessKey\n  type: apiKey\n  in: header\n  parameter: sw-access-key\n  description: Sales channel access key\n  sources:\n  - openapi/shopware-store-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/authentication/shopware-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- E-Commerce
- Open Source
- Headless Commerce
- B2B
- B2C
- REST
- OAuth2
---
