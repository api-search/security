---
api_key_in: []
api_specs:
- filename: arch-accounts-api-openapi.yml
  format: yaml
  label: Arch Accounts API
  slug: arch-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-accounts-api-openapi.yml
- filename: arch-activities-api-openapi.yml
  format: yaml
  label: Arch Activities API
  slug: arch-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-activities-api-openapi.yml
- filename: arch-addepar-api-openapi.yml
  format: yaml
  label: Arch Addepar API
  slug: arch-addepar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-addepar-api-openapi.yml
- filename: arch-authentication-api-openapi.yml
  format: yaml
  label: Arch Authentication API
  slug: arch-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-authentication-api-openapi.yml
- filename: arch-cash-flows-api-openapi.yml
  format: yaml
  label: Arch Cash Flows API
  slug: arch-cash-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-cash-flows-api-openapi.yml
- filename: arch-firms-api-openapi.yml
  format: yaml
  label: Arch Firms API
  slug: arch-firms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-firms-api-openapi.yml
- filename: arch-holdings-api-openapi.yml
  format: yaml
  label: Arch Holdings API
  slug: arch-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-holdings-api-openapi.yml
- filename: arch-investing-entities-api-openapi.yml
  format: yaml
  label: Arch Investing Entities API
  slug: arch-investing-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-investing-entities-api-openapi.yml
- filename: arch-issuing-entities-api-openapi.yml
  format: yaml
  label: Arch Issuing Entities API
  slug: arch-issuing-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-issuing-entities-api-openapi.yml
- filename: arch-lookthroughs-api-openapi.yml
  format: yaml
  label: Arch Lookthroughs API
  slug: arch-lookthroughs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-lookthroughs-api-openapi.yml
- filename: arch-offerings-api-openapi.yml
  format: yaml
  label: Arch Offerings API
  slug: arch-offerings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-offerings-api-openapi.yml
- filename: arch-tasks-api-openapi.yml
  format: yaml
  label: Arch Tasks API
  slug: arch-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-tasks-api-openapi.yml
- filename: arch-tax-documents-api-openapi.yml
  format: yaml
  label: Arch Tax Documents API
  slug: arch-tax-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-tax-documents-api-openapi.yml
- filename: arch-user-roles-api-openapi.yml
  format: yaml
  label: Arch User Roles API
  slug: arch-user-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-user-roles-api-openapi.yml
- filename: arch-users-api-openapi.yml
  format: yaml
  label: Arch Users API
  slug: arch-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/openapi/arch-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Arch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arch
provider_slug: arch
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/arch-client-api-openapi.json
  type: http
slug: arch-authentication
source_filename: arch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/arch-client-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/arch-client-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arch/refs/heads/main/authentication/arch-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Private Markets
- Alternative Investments
- Fintech
- Wealth Management
- Investment Administration
- Portfolio Management
- Documents
---
