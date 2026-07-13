---
api_key_in: []
api_specs:
- filename: scotiabank-tranxact-openapi.yml
  format: yaml
  label: Scotia TranXact APIs
  slug: scotia-tranxact
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-tranxact-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Scotiabank Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Scotiabank secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Scotiabank
provider_slug: scotiabank
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://developer.api.scotiabank.com/auth/token
  name: OAuth2
  sources:
  - openapi/scotiabank-tranxact-openapi.yml
  type: oauth2
slug: scotiabank-authentication
source_filename: scotiabank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scotiabank-tranxact-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.scotiabank.com/auth/token\n    scopes: 3\n  sources:\n  - openapi/scotiabank-tranxact-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/authentication/scotiabank-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Banking
- Finance
- Payments
- Canada
- Open Banking
---
