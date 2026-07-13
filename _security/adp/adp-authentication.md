---
api_key_in: []
api_specs:
- filename: adp-workers-openapi.yml
  format: yaml
  label: ADP Workers API
  slug: adp-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/openapi/adp-workers-openapi.yml
- filename: adp-payroll-openapi.yml
  format: yaml
  label: ADP Payroll API
  slug: adp-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/openapi/adp-payroll-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Adp Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: ADP secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: ADP
provider_slug: adp
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://accounts.adp.com/auth/oauth/v2/token
  name: oauth2ClientCredentials
  sources:
  - openapi/adp-payroll-openapi.yml
  - openapi/adp-workers-openapi.yml
  type: oauth2
slug: adp-authentication
source_filename: adp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adp-payroll-openapi.yml, openapi/adp-workers-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.adp.com/auth/oauth/v2/token\n    scopes: 1\n  sources:\n  - openapi/adp-payroll-openapi.yml\n  - openapi/adp-workers-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/authentication/adp-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
---
