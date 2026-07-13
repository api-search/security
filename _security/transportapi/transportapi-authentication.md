---
api_key_in:
- header
api_specs:
- filename: transportapi-openapi.yml
  format: yaml
  label: TransportAPI
  slug: transportapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transportapi/refs/heads/main/openapi/transportapi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Transportapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: TransportAPI secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TransportAPI
provider_slug: transportapi
scheme_count: 2
schemes:
- description: Application ID header
  in: header
  name: AppIdAuth
  parameter: X-App-Id
  sources:
  - openapi/transportapi-openapi.yml
  type: apiKey
- description: Application key header
  in: header
  name: AppKeyAuth
  parameter: X-App-Key
  sources:
  - openapi/transportapi-openapi.yml
  type: apiKey
slug: transportapi-authentication
source_filename: transportapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/transportapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AppIdAuth\n  type: apiKey\n  in: header\n  parameter: X-App-Id\n  description: Application ID header\n  sources:\n  - openapi/transportapi-openapi.yml\n- name: AppKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-App-Key\n  description: Application key header\n  sources:\n  - openapi/transportapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transportapi/refs/heads/main/authentication/transportapi-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Public Transit
- Transport
- UK
- Real-Time
- Journey Planning
- Bus
- Rail
---
