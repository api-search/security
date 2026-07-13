---
api_key_in:
- header
api_specs:
- filename: multiplier-openapi.yml
  format: yaml
  label: Multiplier Members API
  slug: members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/openapi/multiplier-openapi.yml
- filename: multiplier-openapi.yml
  format: yaml
  label: Multiplier Contracts API
  slug: contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/openapi/multiplier-openapi.yml
- filename: multiplier-openapi.yml
  format: yaml
  label: Multiplier Payroll API
  slug: payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/openapi/multiplier-openapi.yml
- filename: multiplier-openapi.yml
  format: yaml
  label: Multiplier Payments API
  slug: payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/openapi/multiplier-openapi.yml
- filename: multiplier-openapi.yml
  format: yaml
  label: Multiplier Time Off API
  slug: time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/openapi/multiplier-openapi.yml
- filename: multiplier-openapi.yml
  format: yaml
  label: Multiplier Invoices API
  slug: invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/openapi/multiplier-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Multiplier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Multiplier secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Multiplier
provider_slug: multiplier
scheme_count: 1
schemes:
- description: Service User API token created by an account administrator in Multiplier's Configuration area and supplied in the Authorization header. Tokens are scoped to the account and its enabled integrations.
  in: header
  name: ServiceUserToken
  parameter: Authorization
  sources:
  - openapi/multiplier-openapi.yml
  type: apiKey
slug: multiplier-authentication
source_filename: multiplier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/multiplier-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ServiceUserToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Service User API token created by an account administrator in Multiplier's Configuration\n    area and supplied in the Authorization header. Tokens are scoped to the account and its\n    enabled integrations.\n  sources:\n  - openapi/multiplier-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/authentication/multiplier-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- EOR
- Global Employment
- Payroll
- HR
- Contractors
---
