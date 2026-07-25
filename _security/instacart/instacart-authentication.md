---
api_key_in:
- header
api_specs:
- filename: instacart-authentication-api-openapi.yml
  format: yaml
  label: instacart Authentication API
  slug: instacart-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-authentication-api-openapi.yml
- filename: instacart-chat-api-openapi.yml
  format: yaml
  label: instacart Chat API
  slug: instacart-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-chat-api-openapi.yml
- filename: instacart-delivery-api-openapi.yml
  format: yaml
  label: instacart Delivery API
  slug: instacart-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-delivery-api-openapi.yml
- filename: instacart-items-api-openapi.yml
  format: yaml
  label: instacart Items API
  slug: instacart-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-items-api-openapi.yml
- filename: instacart-last-mile-delivery-api-openapi.yml
  format: yaml
  label: instacart Last Mile Delivery API
  slug: instacart-last-mile-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-last-mile-delivery-api-openapi.yml
- filename: instacart-orders-api-openapi.yml
  format: yaml
  label: instacart Orders API
  slug: instacart-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-orders-api-openapi.yml
- filename: instacart-pickup-api-openapi.yml
  format: yaml
  label: instacart Pickup API
  slug: instacart-pickup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-pickup-api-openapi.yml
- filename: instacart-products-api-openapi.yml
  format: yaml
  label: instacart Products API
  slug: instacart-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-products-api-openapi.yml
- filename: instacart-replacements-api-openapi.yml
  format: yaml
  label: instacart Replacements API
  slug: instacart-replacements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-replacements-api-openapi.yml
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
