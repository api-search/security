---
api_key_in:
- header
api_specs:
- filename: openapi3.json
  format: json
  label: Convoy API
  slug: convoy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/frain-dev/convoy/main/docs/v3/openapi3.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Convoy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convoy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Convoy
provider_slug: convoy
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/convoy-openapi.yml
  type: apiKey
slug: convoy-authentication
source_filename: convoy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/convoy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/convoy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/authentication/convoy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Webhooks
- Webhook Gateway
- Event Delivery
- Eventing
- Messaging
- Integration
- API Infrastructure
---
