---
anonymous_access: false
api_key_in: []
api_specs:
- filename: wisdomtree-accruals-api-openapi.yml
  format: yaml
  label: WisdomTree Accruals API
  slug: wisdomtree-accruals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-accruals-api-openapi.yml
- filename: wisdomtree-dividend-payment-preferences-api-openapi.yml
  format: yaml
  label: WisdomTree Dividend Payment Preferences API
  slug: wisdomtree-dividend-payment-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-dividend-payment-preferences-api-openapi.yml
- filename: wisdomtree-fund-data-api-openapi.yml
  format: yaml
  label: WisdomTree Fund Data API
  slug: wisdomtree-fund-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-fund-data-api-openapi.yml
- filename: wisdomtree-orders-api-openapi.yml
  format: yaml
  label: WisdomTree Orders API
  slug: wisdomtree-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-orders-api-openapi.yml
- filename: wisdomtree-organizations-api-openapi.yml
  format: yaml
  label: WisdomTree Organizations API
  slug: wisdomtree-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-organizations-api-openapi.yml
- filename: wisdomtree-statements-api-openapi.yml
  format: yaml
  label: WisdomTree Statements API
  slug: wisdomtree-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-statements-api-openapi.yml
- filename: wisdomtree-users-api-openapi.yml
  format: yaml
  label: WisdomTree Users API
  slug: wisdomtree-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-users-api-openapi.yml
- filename: wisdomtree-wallets-api-openapi.yml
  format: yaml
  label: WisdomTree Wallets API
  slug: wisdomtree-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-wallets-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Wisdomtree Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: WisdomTree secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: WisdomTree
provider_slug: wisdomtree
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 3
    tokenUrl: https://app.wisdomtreeconnect.com/o/token/
  name: oauth2
  sources:
  - openapi/wisdomtree-connect-openapi.yml
  type: oauth2
slug: wisdomtree-authentication
source_filename: wisdomtree-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/wisdomtree-connect-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://app.wisdomtreeconnect.com/o/token/\n    scopes: 3\n  sources:\n  - openapi/wisdomtree-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/authentication/wisdomtree-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Asset Management
- ETFs
- Tokenization
- Tokenized Funds
- Financial Services
- Fund Data
---
