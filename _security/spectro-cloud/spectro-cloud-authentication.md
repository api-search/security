---
api_key_in:
- header
api_specs:
- filename: spectro-cloud-palette-openapi.json
  format: json
  label: Palette APIs
  slug: palette-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spectro-cloud/refs/heads/main/openapi/spectro-cloud-palette-openapi.json
- filename: spectro-cloud-edge-management-openapi.json
  format: json
  label: Edge Local Management APIs
  slug: edge-local-management-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spectro-cloud/refs/heads/main/openapi/spectro-cloud-edge-management-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spectro Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spectro Cloud secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Spectro Cloud
provider_slug: spectro-cloud
scheme_count: 2
schemes:
- description: JWT authorization token obtained using /v1/users/default/login API
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/spectro-cloud-edge-management-openapi.json
  - openapi/spectro-cloud-palette-openapi.json
  type: apiKey
- description: API key authorization where API key can be generated from Palette console under Profile > My API Keys
  in: header
  name: ApiKey
  parameter: ApiKey
  sources:
  - openapi/spectro-cloud-palette-openapi.json
  type: apiKey
slug: spectro-cloud-authentication
source_filename: spectro-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/spectro-cloud-edge-management-openapi.json, openapi/spectro-cloud-palette-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: JWT authorization token obtained using /v1/users/default/login API\n  sources:\n  - openapi/spectro-cloud-edge-management-openapi.json\n  - openapi/spectro-cloud-palette-openapi.json\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: ApiKey\n  description: API key authorization where API key can be generated from Palette console under\n    Profile > My API Keys\n  sources:\n  - openapi/spectro-cloud-palette-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spectro-cloud/refs/heads/main/authentication/spectro-cloud-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Infrastructure
- Kubernetes
- Cloud Native
- Cluster Management
- Edge Computing
- Multi-Cloud
- DevOps
- AI Infrastructure
---
