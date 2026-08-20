---
api_key_in: []
api_specs:
- filename: ramp-accounts-api-openapi.yml
  format: yaml
  label: Ramp Accounts API
  slug: ramp-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-accounts-api-openapi.yml
- filename: ramp-audit-logs-api-openapi.yml
  format: yaml
  label: Ramp Audit Logs API
  slug: ramp-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-audit-logs-api-openapi.yml
- filename: ramp-bills-api-openapi.yml
  format: yaml
  label: Ramp Bills API
  slug: ramp-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-bills-api-openapi.yml
- filename: ramp-cards-api-openapi.yml
  format: yaml
  label: Ramp Cards API
  slug: ramp-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-cards-api-openapi.yml
- filename: ramp-departments-api-openapi.yml
  format: yaml
  label: Ramp Departments API
  slug: ramp-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-departments-api-openapi.yml
- filename: ramp-locations-api-openapi.yml
  format: yaml
  label: Ramp Locations API
  slug: ramp-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-locations-api-openapi.yml
- filename: ramp-reimbursements-api-openapi.yml
  format: yaml
  label: Ramp Reimbursements API
  slug: ramp-reimbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-reimbursements-api-openapi.yml
- filename: ramp-statements-api-openapi.yml
  format: yaml
  label: Ramp Statements API
  slug: ramp-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-statements-api-openapi.yml
- filename: ramp-transactions-api-openapi.yml
  format: yaml
  label: Ramp Transactions API
  slug: ramp-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-transactions-api-openapi.yml
- filename: ramp-users-api-openapi.yml
  format: yaml
  label: Ramp Users API
  slug: ramp-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-users-api-openapi.yml
- filename: ramp-vendors-api-openapi.yml
  format: yaml
  label: Ramp Vendors API
  slug: ramp-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-vendors-api-openapi.yml
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
- Reimbursement
---
