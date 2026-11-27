---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: hairdora-com-appointments-api-openapi.yml
  format: yaml
  label: HairDora Appointments API
  slug: hairdora-com-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hairdora-com/openapi/hairdora-com-appointments-api-openapi.yml
- filename: hairdora-com-clients-api-openapi.yml
  format: yaml
  label: HairDora Clients API
  slug: hairdora-com-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hairdora-com/openapi/hairdora-com-clients-api-openapi.yml
- filename: hairdora-com-keys-api-openapi.yml
  format: yaml
  label: HairDora Keys API
  slug: hairdora-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hairdora-com/openapi/hairdora-com-keys-api-openapi.yml
- filename: hairdora-com-salons-api-openapi.yml
  format: yaml
  label: HairDora Salons API
  slug: hairdora-com-salons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hairdora-com/openapi/hairdora-com-salons-api-openapi.yml
- filename: hairdora-com-services-api-openapi.yml
  format: yaml
  label: HairDora Services API
  slug: hairdora-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hairdora-com/openapi/hairdora-com-services-api-openapi.yml
- filename: hairdora-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: HairDora Webhook subscriptions API
  slug: hairdora-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hairdora-com/openapi/hairdora-com-webhook-subscriptions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: HairDora Authentication
name_suffix: Authentication
oauth_flows: []
overview: HairDora secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HairDora
provider_slug: hairdora-com
scheme_count: 2
schemes:
- description: 'HTTP Basic auth carrying only the API key secret: Authorization: Basic base64(<key secret>).'
  name: apiKey
  scheme: basic
  sources:
  - openapi/hairdora-com-openapi.json
  type: http
- description: 'Operator session token issued by the HairDora dashboard: Authorization: Token <access token>.'
  in: header
  name: accessToken
  parameter: Authorization
  sources:
  - openapi/hairdora-com-openapi.json
  type: apiKey
slug: hairdora-com-authentication
source_filename: hairdora-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hairdora-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: http\n  scheme: basic\n  description: 'HTTP Basic auth carrying only the API key secret: Authorization: Basic base64(<key\n    secret>).'\n  sources:\n  - openapi/hairdora-com-openapi.json\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Operator session token issued by the HairDora dashboard: Authorization: Token\n    <access token>.'\n  sources:\n  - openapi/hairdora-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hairdora-com/authentication/hairdora-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Salon
- Software
- Management
- Booking
- Hair
---
