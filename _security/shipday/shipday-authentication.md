---
api_key_in: []
api_specs:
- filename: shipday-openapi.yml
  format: yaml
  label: Shipday Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-openapi.yml
- filename: shipday-openapi.yml
  format: yaml
  label: Shipday Drivers / Carriers API
  slug: drivers-carriers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-openapi.yml
- filename: shipday-openapi.yml
  format: yaml
  label: Shipday Order Assignment API
  slug: order-assignment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-openapi.yml
- filename: shipday-openapi.yml
  format: yaml
  label: Shipday On-Demand Delivery API
  slug: on-demand-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-openapi.yml
- filename: shipday-openapi.yml
  format: yaml
  label: Shipday Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shipday Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shipday secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shipday
provider_slug: shipday
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication. Send your API key as the credential in the Authorization header, e.g. `Authorization: Basic {API_KEY}`.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/shipday-openapi.yml
  type: http
slug: shipday-authentication
source_filename: shipday-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shipday-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic authentication. Send your API key as the credential in the Authorization\n    header, e.g. `Authorization: Basic {API_KEY}`.'\n  sources:\n  - openapi/shipday-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/authentication/shipday-authentication.yml
summary_line: http · 1 scheme
tags:
- Delivery
- Logistics
- Last Mile
- Local Delivery
- Dispatch
---
