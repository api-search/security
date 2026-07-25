---
api_key_in:
- header
api_specs:
- filename: nops-essentials-scheduler-api-openapi.yml
  format: yaml
  label: nOps Essentials Scheduler API
  slug: nops-essentials-scheduler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/openapi/nops-essentials-scheduler-api-openapi.yml
- filename: nops-map-migration-api-openapi.yml
  format: yaml
  label: nOps MAP Migration API
  slug: nops-map-migration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/openapi/nops-map-migration-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nops Authentication
name_suffix: Authentication
oauth_flows: []
overview: nOps secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: nOps
provider_slug: nops
scheme_count: 2
schemes:
- description: API key generated from the nOps console under Organization Settings. Include this key in the X-Nops-Api-Key header for all requests.
  in: header
  name: ApiKeyAuth
  parameter: X-Nops-Api-Key
  sources:
  - openapi/nops-nops-openapi.yml
  type: apiKey
- description: Encoded signature for enhanced security. Created using a public/private key pair configured in the nOps console.
  in: header
  name: SignatureAuth
  parameter: x-nops-signature
  sources:
  - openapi/nops-nops-openapi.yml
  type: apiKey
slug: nops-authentication
source_filename: nops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nops-nops-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Nops-Api-Key\n  description: API key generated from the nOps console under Organization Settings. Include\n    this key in the X-Nops-Api-Key header for all requests.\n  sources:\n  - openapi/nops-nops-openapi.yml\n- name: SignatureAuth\n  type: apiKey\n  in: header\n  parameter: x-nops-signature\n  description: Encoded signature for enhanced security. Created using a public/private key pair\n    configured in the nOps console.\n  sources:\n  - openapi/nops-nops-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/authentication/nops-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Costs
- FinOps
---
