---
api_key_in: []
api_specs:
- filename: shell-b2b-mobility-openapi.yml
  format: yaml
  label: Shell B2B Mobility Card Management API
  slug: b2b-mobility-card-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-b2b-mobility-openapi.yml
- filename: shell-b2b-mobility-openapi.yml
  format: yaml
  label: Shell B2B Mobility Card Transaction Data API
  slug: b2b-mobility-card-transaction-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-b2b-mobility-openapi.yml
- filename: shell-b2b-mobility-openapi.yml
  format: yaml
  label: Shell B2B Mobility Invoice API
  slug: b2b-mobility-invoice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-b2b-mobility-openapi.yml
- filename: shell-loyalty-openapi.yml
  format: yaml
  label: Shell Loyalty Catalogue API
  slug: loyalty-catalogue
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-loyalty-openapi.yml
- filename: shell-loyalty-openapi.yml
  format: yaml
  label: Shell Loyalty Account Management API
  slug: loyalty-account-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-loyalty-openapi.yml
- filename: shell-loyalty-openapi.yml
  format: yaml
  label: Shell Loyalty Points Balance API
  slug: loyalty-points-balance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-loyalty-openapi.yml
- filename: shell-loyalty-openapi.yml
  format: yaml
  label: Shell Loyalty Points Redemption API
  slug: loyalty-points-redemption
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-loyalty-openapi.yml
- filename: shell-lubricants-openapi.yml
  format: yaml
  label: Shell Lubricants Order Management API
  slug: lubricants-order-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-lubricants-openapi.yml
- filename: shell-b2b-mobility-openapi.yml
  format: yaml
  label: Shell B2B Mobility Sites API
  slug: b2b-mobility-sites
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-b2b-mobility-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Shell Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Shell secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Shell
provider_slug: shell
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://api.shell.com/oauth/token
  name: OAuth2
  sources:
  - openapi/shell-b2b-mobility-openapi.yml
  - openapi/shell-loyalty-openapi.yml
  - openapi/shell-lubricants-openapi.yml
  type: oauth2
slug: shell-authentication
source_filename: shell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shell-b2b-mobility-openapi.yml, openapi/shell-loyalty-openapi.yml, openapi/shell-lubricants-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.shell.com/oauth/token\n    scopes: 4\n  sources:\n  - openapi/shell-b2b-mobility-openapi.yml\n  - openapi/shell-loyalty-openapi.yml\n  - openapi/shell-lubricants-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/authentication/shell-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Aviation
- Electric Vehicle Charging
- Energy
- Fleet Management
- Fuel
- Gas
- Loyalty
- Lubricants
- Mobility
- Oil and Gas
- Renewable Energy
---
