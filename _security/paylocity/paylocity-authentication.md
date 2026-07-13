---
api_key_in: []
api_specs:
- filename: paylocity-openapi.yml
  format: yaml
  label: Paylocity Integrations REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paylocity/refs/heads/main/openapi/paylocity-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Paylocity Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Paylocity secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Paylocity
provider_slug: paylocity
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials grant. Credentials are provisioned by Paylocity.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.paylocity.com/IdentityServer/connect/token
  name: oauth2ClientCredentials
  sources:
  - openapi/paylocity-openapi.yml
  type: oauth2
slug: paylocity-authentication
source_filename: paylocity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paylocity-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.paylocity.com/IdentityServer/connect/token\n    scopes: 0\n  description: OAuth 2.0 client credentials grant. Credentials are provisioned by Paylocity.\n  sources:\n  - openapi/paylocity-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paylocity/refs/heads/main/authentication/paylocity-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- HR
- Payroll
- HCM
- Benefits
- Workforce Management
- Time Tracking
---
