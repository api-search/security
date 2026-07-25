---
api_key_in: []
api_specs:
- filename: shell-accounts-api-openapi.yml
  format: yaml
  label: Shell Accounts API
  slug: shell-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-accounts-api-openapi.yml
- filename: shell-cards-api-openapi.yml
  format: yaml
  label: Shell Cards API
  slug: shell-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-cards-api-openapi.yml
- filename: shell-catalogue-api-openapi.yml
  format: yaml
  label: Shell Catalogue API
  slug: shell-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-catalogue-api-openapi.yml
- filename: shell-invoices-api-openapi.yml
  format: yaml
  label: Shell Invoices API
  slug: shell-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-invoices-api-openapi.yml
- filename: shell-limits-api-openapi.yml
  format: yaml
  label: Shell Limits API
  slug: shell-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-limits-api-openapi.yml
- filename: shell-offers-api-openapi.yml
  format: yaml
  label: Shell Offers API
  slug: shell-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-offers-api-openapi.yml
- filename: shell-orders-api-openapi.yml
  format: yaml
  label: Shell Orders API
  slug: shell-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-orders-api-openapi.yml
- filename: shell-points-api-openapi.yml
  format: yaml
  label: Shell Points API
  slug: shell-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-points-api-openapi.yml
- filename: shell-products-api-openapi.yml
  format: yaml
  label: Shell Products API
  slug: shell-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-products-api-openapi.yml
- filename: shell-sites-api-openapi.yml
  format: yaml
  label: Shell Sites API
  slug: shell-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-sites-api-openapi.yml
- filename: shell-transactions-api-openapi.yml
  format: yaml
  label: Shell Transactions API
  slug: shell-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-transactions-api-openapi.yml
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
