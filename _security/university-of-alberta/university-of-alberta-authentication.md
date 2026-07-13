---
api_key_in:
- header
api_specs:
- filename: university-of-alberta-borealis-dataverse.yaml
  format: yaml
  label: University of Alberta Research Data (Borealis Dataverse) API
  slug: borealis-dataverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-alberta/refs/heads/main/openapi/university-of-alberta-borealis-dataverse.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: University Of Alberta Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Alberta secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Alberta
provider_slug: university-of-alberta
scheme_count: 1
schemes:
- description: API token required only for account-scoped or write operations. Public search and info endpoints do not require it.
  in: header
  name: DataverseApiKey
  parameter: X-Dataverse-key
  sources:
  - openapi/university-of-alberta-borealis-dataverse.yaml
  type: apiKey
slug: university-of-alberta-authentication
source_filename: university-of-alberta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-alberta-borealis-dataverse.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: DataverseApiKey\n  type: apiKey\n  in: header\n  parameter: X-Dataverse-key\n  description: API token required only for account-scoped or write operations. Public search\n    and info endpoints do not require it.\n  sources:\n  - openapi/university-of-alberta-borealis-dataverse.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-alberta/refs/heads/main/authentication/university-of-alberta-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- Library
- Canada
---
