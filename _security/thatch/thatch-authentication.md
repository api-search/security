---
api_key_in: []
api_specs:
- filename: thatch-partners-openapi.yml
  format: yaml
  label: Thatch for Platforms API
  slug: thatch-for-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thatch/refs/heads/main/openapi/thatch-partners-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Thatch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thatch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Thatch
provider_slug: thatch
scheme_count: 1
schemes:
- description: 'All requests are authenticated with your API key using Bearer token authentication. Include the header `Authorization: Bearer <YOUR_API_KEY>`. Generate an API key in the Thatch dashboard.'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/thatch-partners-openapi.yml
  type: http
slug: thatch-authentication
source_filename: thatch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/thatch-partners-openapi.yml\ndocs: https://docs.thatch.com/\nsummary:\n  model: All requests are authenticated and authorized using a partner API key sent as a Bearer token. Generate an API key in the Thatch dashboard. Access is limited to approved partners.\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: 'All requests are authenticated with your API key using Bearer token authentication.\n    Include the header `Authorization: Bearer <YOUR_API_KEY>`. Generate an API key in the Thatch\n    dashboard.'\n  sources:\n  - openapi/thatch-partners-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thatch/refs/heads/main/authentication/thatch-authentication.yml
summary_line: http · 1 scheme
tags:
- Health Insurance
- Health Benefits
- ICHRA
- Employee Benefits
- Payroll
- Insurance
- Fintech
- Embedded Finance
- Company
---
