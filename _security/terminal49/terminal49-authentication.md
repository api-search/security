---
api_key_in:
- header
api_specs:
- filename: terminal49-openapi.yml
  format: yaml
  label: Terminal49 Tracking Requests API
  slug: tracking-requests
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/openapi/terminal49-openapi.yml
- filename: terminal49-openapi.yml
  format: yaml
  label: Terminal49 Shipments API
  slug: shipments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/openapi/terminal49-openapi.yml
- filename: terminal49-openapi.yml
  format: yaml
  label: Terminal49 Containers API
  slug: containers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/openapi/terminal49-openapi.yml
- filename: terminal49-openapi.yml
  format: yaml
  label: Terminal49 Transport Events API
  slug: transport-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/openapi/terminal49-openapi.yml
- filename: terminal49-openapi.yml
  format: yaml
  label: Terminal49 Terminals & Shipping Lines API
  slug: terminals-shipping-lines
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/openapi/terminal49-openapi.yml
- filename: terminal49-openapi.yml
  format: yaml
  label: Terminal49 Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/openapi/terminal49-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Terminal49 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terminal49 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Terminal49
provider_slug: terminal49
scheme_count: 1
schemes:
- description: 'Token-based authentication. Send the header `Authorization: Token YOUR_API_KEY`.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/terminal49-openapi.yml
  type: apiKey
slug: terminal49-authentication
source_filename: terminal49-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/terminal49-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token-based authentication. Send the header `Authorization: Token YOUR_API_KEY`.'\n  sources:\n  - openapi/terminal49-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terminal49/refs/heads/main/authentication/terminal49-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Container Tracking
- Ocean Freight
- Supply Chain
- Logistics
- Shipping
---
