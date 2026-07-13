---
api_key_in: []
api_specs:
- filename: fis-payments-openapi.yml
  format: yaml
  label: FIS Payments API
  slug: fis-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-payments-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Fis Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: FIS Global secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: FIS Global
provider_slug: fis
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://api.fisglobal.com/oauth/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/fis-payments-openapi.yml
  type: oauth2
slug: fis-authentication
source_filename: fis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fis-payments-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.fisglobal.com/oauth/token\n    scopes: 3\n  sources:\n  - openapi/fis-payments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/authentication/fis-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Banking
- Core Banking
- Financial Services
- Payments
- Fintech
---
