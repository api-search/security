---
api_key_in:
- header
api_specs:
- filename: elsevier-openapi.yml
  format: yaml
  label: Elsevier Scopus APIs
  slug: elsevier-scopus-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Elsevier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elsevier secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Elsevier
provider_slug: elsevier
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-ELS-APIKey
  sources:
  - openapi/elsevier-openapi.yml
  type: apiKey
slug: elsevier-authentication
source_filename: elsevier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elsevier-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-ELS-APIKey\n  sources:\n  - openapi/elsevier-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/authentication/elsevier-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Content
- Journals
- Medical
- Research
- Scientific
- Technical
---
