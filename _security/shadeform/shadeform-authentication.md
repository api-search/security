---
api_key_in:
- header
api_specs:
- filename: shadeform-openapi.yml
  format: yaml
  label: Shadeform Instances API
  slug: shadeform-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shadeform/refs/heads/main/openapi/shadeform-openapi.yml
- filename: shadeform-openapi.yml
  format: yaml
  label: Shadeform Instance Types & Availability API
  slug: shadeform-instance-types-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shadeform/refs/heads/main/openapi/shadeform-openapi.yml
- filename: shadeform-openapi.yml
  format: yaml
  label: Shadeform Templates API
  slug: shadeform-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shadeform/refs/heads/main/openapi/shadeform-openapi.yml
- filename: shadeform-openapi.yml
  format: yaml
  label: Shadeform Volumes API
  slug: shadeform-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shadeform/refs/heads/main/openapi/shadeform-openapi.yml
- filename: shadeform-openapi.yml
  format: yaml
  label: Shadeform SSH Keys API
  slug: shadeform-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shadeform/refs/heads/main/openapi/shadeform-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shadeform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shadeform secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shadeform
provider_slug: shadeform
scheme_count: 1
schemes:
- description: API key issued from the Shadeform dashboard.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/shadeform-openapi.yml
  type: apiKey
slug: shadeform-authentication
source_filename: shadeform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shadeform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key issued from the Shadeform dashboard.\n  sources:\n  - openapi/shadeform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shadeform/refs/heads/main/authentication/shadeform-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- GPU
- Cloud
- Marketplace
- Compute
- Infrastructure
- AI
---
