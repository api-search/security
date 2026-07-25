---
api_key_in:
- header
- query
api_specs:
- filename: mobileapi-dev-api-api-openapi.yml
  format: yaml
  label: MobileAPI.dev api API
  slug: mobileapi-dev-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-api-api-openapi.yml
- filename: mobileapi-dev-api-token-auth-api-openapi.yml
  format: yaml
  label: MobileAPI.dev api-token-auth API
  slug: mobileapi-dev-api-token-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-api-token-auth-api-openapi.yml
- filename: mobileapi-dev-demo-x7k9m2p4-api-openapi.yml
  format: yaml
  label: MobileAPI.dev demo-x7k9m2p4 API
  slug: mobileapi-dev-demo-x7k9m2p4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-demo-x7k9m2p4-api-openapi.yml
- filename: mobileapi-dev-devices-api-openapi.yml
  format: yaml
  label: MobileAPI.dev devices API
  slug: mobileapi-dev-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-devices-api-openapi.yml
- filename: mobileapi-dev-images-api-openapi.yml
  format: yaml
  label: MobileAPI.dev images API
  slug: mobileapi-dev-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-images-api-openapi.yml
- filename: mobileapi-dev-manufacturers-api-openapi.yml
  format: yaml
  label: MobileAPI.dev manufacturers API
  slug: mobileapi-dev-manufacturers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-manufacturers-api-openapi.yml
- filename: mobileapi-dev-me-api-openapi.yml
  format: yaml
  label: MobileAPI.dev me API
  slug: mobileapi-dev-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-me-api-openapi.yml
- filename: mobileapi-dev-payment-successful-api-openapi.yml
  format: yaml
  label: MobileAPI.dev payment_successful API
  slug: mobileapi-dev-payment-successful-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-payment-successful-api-openapi.yml
- filename: mobileapi-dev-status-api-openapi.yml
  format: yaml
  label: MobileAPI.dev status API
  slug: mobileapi-dev-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-status-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mobileapi Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: MobileAPI.dev secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MobileAPI.dev
provider_slug: mobileapi-dev
scheme_count: 2
schemes:
- description: Provide your API key in the Authorization header using either 'Token YOUR_API_KEY' or 'Bearer [example key]'. Both formats are equivalent.
  in: header
  name: ApiKeyHeader
  parameter: Authorization
  sources:
  - openapi/mobileapi-openapi.yml
  type: apiKey
- description: Fallback - supply your API key as the 'key' query parameter.
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/mobileapi-openapi.yml
  type: apiKey
slug: mobileapi-dev-authentication
source_filename: mobileapi-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mobileapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Provide your API key in the Authorization header using either 'Token YOUR_API_KEY'\n    or 'Bearer [example key]'. Both formats are equivalent.\n  sources:\n  - openapi/mobileapi-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: Fallback - supply your API key as the 'key' query parameter.\n  sources:\n  - openapi/mobileapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/authentication/mobileapi-dev-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Data API
- Developer Tools
- Device Specifications
- Mobile Data
- Phone Specs
- REST API
- SaaS
---
