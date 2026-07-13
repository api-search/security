---
api_key_in:
- header
api_specs:
- filename: wageningen-university-research-agrodatacube-v2.yaml
  format: yaml
  label: AgroDataCube API v2
  slug: agrodatacube-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wageningen-university-research/refs/heads/main/openapi/wageningen-university-research-agrodatacube-v2.yaml
- filename: wageningen-university-research-agrodatacube-v1.yaml
  format: yaml
  label: AgroDataCube API v1 (legacy)
  slug: agrodatacube-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wageningen-university-research/refs/heads/main/openapi/wageningen-university-research-agrodatacube-v1.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wageningen University Research Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wageningen University & Research secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wageningen University & Research
provider_slug: wageningen-university-research
scheme_count: 1
schemes:
- description: Access token obtained via https://agrodatacube.wur.nl/api/register.jsp
  in: header
  name: tokenHeader
  parameter: token
  sources:
  - openapi/wageningen-university-research-agrodatacube-v1.yaml
  - openapi/wageningen-university-research-agrodatacube-v2.yaml
  type: apiKey
slug: wageningen-university-research-authentication
source_filename: wageningen-university-research-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wageningen-university-research-agrodatacube-v1.yaml, openapi/wageningen-university-research-agrodatacube-v2.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenHeader\n  type: apiKey\n  in: header\n  parameter: token\n  description: Access token obtained via https://agrodatacube.wur.nl/api/register.jsp\n  sources:\n  - openapi/wageningen-university-research-agrodatacube-v1.yaml\n  - openapi/wageningen-university-research-agrodatacube-v2.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wageningen-university-research/refs/heads/main/authentication/wageningen-university-research-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Agriculture
- Agri-Food
- Open Data
- Netherlands
---
