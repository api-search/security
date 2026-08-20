---
api_key_in:
- header
api_specs:
- filename: tickitto-authentication-api-openapi.yml
  format: yaml
  label: Tickitto Authentication API
  slug: tickitto-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-authentication-api-openapi.yml
- filename: tickitto-availability-api-openapi.yml
  format: yaml
  label: Tickitto Availability API
  slug: tickitto-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-availability-api-openapi.yml
- filename: tickitto-basket-api-openapi.yml
  format: yaml
  label: Tickitto Basket API
  slug: tickitto-basket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-basket-api-openapi.yml
- filename: tickitto-events-api-openapi.yml
  format: yaml
  label: Tickitto Events API
  slug: tickitto-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-events-api-openapi.yml
- filename: tickitto-metadata-api-openapi.yml
  format: yaml
  label: Tickitto Metadata API
  slug: tickitto-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-metadata-api-openapi.yml
- filename: tickitto-search-api-openapi.yml
  format: yaml
  label: Tickitto Search API
  slug: tickitto-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-search-api-openapi.yml
- filename: tickitto-system-status-api-openapi.yml
  format: yaml
  label: Tickitto System Status API
  slug: tickitto-system-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-system-status-api-openapi.yml
- filename: tickitto-webhooks-api-openapi.yml
  format: yaml
  label: Tickitto Webhooks API
  slug: tickitto-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/openapi/tickitto-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tickitto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tickitto secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tickitto
provider_slug: tickitto
scheme_count: 2
schemes:
- in: header
  name: APIKeyHeader
  parameter: key
  sources:
  - openapi/tickitto-openapi-original.json
  type: apiKey
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/tickitto-openapi-original.json
  type: http
slug: tickitto-authentication
source_filename: tickitto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tickitto-openapi-original.json\ndocs: https://docs.tickitto.com/key-principles/authentication\nnotes: >-\n  Authenticate by sending your API key in the `key` request header (no password). All endpoints\n  require authentication and HTTPS; unauthenticated or plain-HTTP requests fail. Keys are issued\n  by a Tickitto account manager and are tied to your account settings (booking fees, search\n  restrictions). An HTTP bearer scheme is also defined in the spec.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: key\n  sources:\n  - openapi/tickitto-openapi-original.json\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/tickitto-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tickitto/refs/heads/main/authentication/tickitto-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Ticketing
- Event
- Marketplace
- Travel & Experiences
- Entertainment
- Payments
- Commerce
---
