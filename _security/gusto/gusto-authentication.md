---
api_key_in: []
api_specs:
- filename: gusto-asyncapi.yml
  format: yaml
  label: Gusto Embedded Payroll API
  slug: embedded-payroll-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/openapi/gusto-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gusto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gusto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gusto
provider_slug: gusto
scheme_count: 1
schemes:
- description: 'OAuth 2.0 access token for company-level access or system-level bearer

    token for partner operations. Scopes such as payrolls:read, payrolls:run,

    contractors:write provide fine-grained permissions.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gusto-openapi.yml
  type: http
slug: gusto-authentication
source_filename: gusto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gusto-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    OAuth 2.0 access token for company-level access or system-level bearer\n    token for partner operations. Scopes such as payrolls:read, payrolls:run,\n    contractors:write provide fine-grained permissions.\n  sources:\n  - openapi/gusto-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/authentication/gusto-authentication.yml
summary_line: http · 1 scheme
tags:
- Human Resources
- Payroll
- Benefits
- Enterprise Software
- Embedded Finance
---
