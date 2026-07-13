---
api_key_in: []
api_specs:
- filename: guusto-openapi.yml
  format: yaml
  label: Guusto Gifts API
  slug: guusto-gifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guusto/refs/heads/main/openapi/guusto-openapi.yml
- filename: guusto-openapi.yml
  format: yaml
  label: Guusto Account Budget API
  slug: guusto-account-budget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guusto/refs/heads/main/openapi/guusto-openapi.yml
- filename: guusto-openapi.yml
  format: yaml
  label: Guusto Reports API
  slug: guusto-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guusto/refs/heads/main/openapi/guusto-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Guusto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Guusto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Guusto
provider_slug: guusto
scheme_count: 1
schemes:
- description: Bearer API token issued from the Guusto workspace (Premium plan).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/guusto-openapi.yml
  type: http
slug: guusto-authentication
source_filename: guusto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/guusto-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer API token issued from the Guusto workspace (Premium plan).\n  sources:\n  - openapi/guusto-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guusto/refs/heads/main/authentication/guusto-authentication.yml
summary_line: http · 1 scheme
tags:
- Employee Recognition
- Rewards
- Gifting
- Gift Cards
- HR
- Rewards and Recognition
---
