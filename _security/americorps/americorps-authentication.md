---
api_key_in:
- header
api_specs:
- filename: americorps-openapi.yml
  format: yaml
  label: AmeriCorps Open Data SODA API
  slug: americorps-open-data-soda-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/americorps/refs/heads/main/openapi/americorps-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Americorps Authentication
name_suffix: Authentication
oauth_flows: []
overview: AmeriCorps secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AmeriCorps
provider_slug: americorps
scheme_count: 1
schemes:
- description: 'Optional Socrata application token. Anonymous access is allowed, but

    requests without a token are subject to lower throttling limits.'
  in: header
  name: SocrataAppToken
  parameter: X-App-Token
  sources:
  - openapi/americorps-openapi.yml
  type: apiKey
slug: americorps-authentication
source_filename: americorps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/americorps-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SocrataAppToken\n  type: apiKey\n  in: header\n  parameter: X-App-Token\n  description: |-\n    Optional Socrata application token. Anonymous access is allowed, but\n    requests without a token are subject to lower throttling limits.\n  sources:\n  - openapi/americorps-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/americorps/refs/heads/main/authentication/americorps-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal Government
- National Service
- Volunteerism
- Community Development
- Civic Engagement
- Education
- Disaster Response
- Environmental Conservation
---
