---
api_key_in: []
api_specs:
- filename: ramp-developer-api-openapi.yml
  format: yaml
  label: Ramp Developer API
  slug: ramp-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-developer-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ramp Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Ramp secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Ramp
provider_slug: ramp
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 12
    tokenUrl: https://api.ramp.com/developer/v1/token
  name: OAuth2
  sources:
  - openapi/ramp-developer-api-openapi.yml
  type: oauth2
slug: ramp-authentication
source_filename: ramp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ramp-developer-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ramp.com/developer/v1/token\n    scopes: 12\n  sources:\n  - openapi/ramp-developer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/authentication/ramp-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Finance
- Spend Management
- Corporate Cards
- Expense Management
- Accounts Payable
- Bill Pay
- Accounting
- Reimbursements
---
