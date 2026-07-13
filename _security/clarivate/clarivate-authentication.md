---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Clarivate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clarivate secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clarivate
provider_slug: clarivate
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: X-ApiKey
  sources:
  - openapi/clarivate-openapi.yml
  type: apiKey
slug: clarivate-authentication
source_filename: clarivate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clarivate-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-ApiKey\n  sources:\n  - openapi/clarivate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarivate/refs/heads/main/authentication/clarivate-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Citations
- Data
- Drug Pipeline
- Insights
- Intellectual Property
- Life Sciences
- Patents
- Publications
- Research
---
