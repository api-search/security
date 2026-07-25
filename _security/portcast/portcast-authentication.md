---
api_key_in:
- header
api_specs:
- filename: portcast-augmentation-api-openapi.yml
  format: yaml
  label: Portcast Augmentation API
  slug: portcast-augmentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/openapi/portcast-augmentation-api-openapi.yml
- filename: portcast-container-detail-api-openapi.yml
  format: yaml
  label: Portcast Container Detail API
  slug: portcast-container-detail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/openapi/portcast-container-detail-api-openapi.yml
- filename: portcast-reference-api-openapi.yml
  format: yaml
  label: Portcast Reference API
  slug: portcast-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/openapi/portcast-reference-api-openapi.yml
- filename: portcast-tracking-data-api-openapi.yml
  format: yaml
  label: Portcast Tracking Data API
  slug: portcast-tracking-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/openapi/portcast-tracking-data-api-openapi.yml
- filename: portcast-tracking-upload-api-openapi.yml
  format: yaml
  label: Portcast Tracking Upload API
  slug: portcast-tracking-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/openapi/portcast-tracking-upload-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Portcast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Portcast secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Portcast
provider_slug: portcast
scheme_count: 1
schemes:
- description: API key issued by Portcast, sent in the x-api-key request header.
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/portcast-openapi.yml
  type: apiKey
slug: portcast-authentication
source_filename: portcast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/portcast-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key issued by Portcast, sent in the x-api-key request header.\n  sources:\n  - openapi/portcast-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/authentication/portcast-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Supply Chain
- Container Tracking
- Logistics
- Predictive ETA
- Ocean Freight
---
