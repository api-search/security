---
api_key_in: []
api_specs:
- filename: vanta-openapi.yml
  format: yaml
  label: Vanta API
  slug: vanta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-openapi.yml
- filename: vanta-auditor-openapi.yml
  format: yaml
  label: Vanta Auditor API
  slug: vanta-auditor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-auditor-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Vanta Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Vanta secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Vanta
provider_slug: vanta
scheme_count: 2
schemes:
- description: Get an oauth token from the token url and use it as a bearer token to access the Vanta API.
  flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://api.vanta.com/oauth/token
  name: oauth
  sources:
  - openapi/vanta-auditor-openapi.yml
  - openapi/vanta-openapi.yml
  type: oauth2
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vanta-auditor-openapi.yml
  type: http
slug: vanta-authentication
source_filename: vanta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vanta-auditor-openapi.yml, openapi/vanta-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.vanta.com/oauth/token\n    scopes: 4\n  description: Get an oauth token from the token url and use it as a bearer token to access\n    the Vanta API.\n  sources:\n  - openapi/vanta-auditor-openapi.yml\n  - openapi/vanta-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/vanta-auditor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/authentication/vanta-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Cybersecurity
- Compliance
- Security
- Governance
- Risk Management
---
