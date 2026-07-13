---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kevel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kevel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kevel
provider_slug: kevel
scheme_count: 1
schemes:
- description: Management/Reporting API key issued from the Kevel UI.
  in: header
  name: ApiKeyAuth
  parameter: X-Adzerk-ApiKey
  sources:
  - openapi/kevel-openapi.yml
  type: apiKey
slug: kevel-authentication
source_filename: kevel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kevel-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Adzerk-ApiKey\n  description: Management/Reporting API key issued from the Kevel UI.\n  sources:\n  - openapi/kevel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/authentication/kevel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Ad Serving
- Advertising
- API-First
- Audience
- Monetization
- Reporting
---
