---
api_key_in:
- header
api_specs:
- filename: instacart-developer-platform-api-openapi.yml
  format: yaml
  label: Instacart Developer Platform API
  slug: developer-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-developer-platform-api-openapi.yml
- filename: instacart-connect-fulfillment-api-openapi.yml
  format: yaml
  label: Instacart Connect Fulfillment API
  slug: connect-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-connect-fulfillment-api-openapi.yml
- filename: instacart-connect-post-checkout-api-openapi.yml
  format: yaml
  label: Instacart Connect Post-Checkout API
  slug: connect-post-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-connect-post-checkout-api-openapi.yml
- filename: instacart-catalog-api-openapi.yml
  format: yaml
  label: Instacart Catalog API
  slug: catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-catalog-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Instacart Authentication
name_suffix: Authentication
oauth_flows: []
overview: instacart secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: instacart
provider_slug: instacart
scheme_count: 2
schemes:
- description: OAuth 2.0 Bearer token obtained using client credentials with the connect:data_ingestion scope.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/instacart-catalog-api-openapi.yml
  - openapi/instacart-connect-fulfillment-api-openapi.yml
  - openapi/instacart-connect-post-checkout-api-openapi.yml
  type: http
- description: API key authentication. Include your API key in the Authorization header.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/instacart-developer-platform-api-openapi.yml
  type: apiKey
slug: instacart-authentication
source_filename: instacart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/instacart-catalog-api-openapi.yml, openapi/instacart-connect-fulfillment-api-openapi.yml,\n  openapi/instacart-connect-post-checkout-api-openapi.yml, openapi/instacart-developer-platform-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token obtained using client credentials with the connect:data_ingestion\n    scope.\n  sources:\n  - openapi/instacart-catalog-api-openapi.yml\n  - openapi/instacart-connect-fulfillment-api-openapi.yml\n  - openapi/instacart-connect-post-checkout-api-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key authentication. Include your API key in the Authorization header.\n  sources:\n  - openapi/instacart-developer-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/authentication/instacart-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
