---
api_key_in: []
api_specs:
- filename: narmi-public-openapi-original.yml
  format: yaml
  label: Narmi Public API
  slug: narmi-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narmi/refs/heads/main/openapi/narmi-public-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Narmi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Narmi secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Narmi
provider_slug: narmi
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: /v2/oauth/authorize/
    flow: authorizationCode
    scopes: 9
    tokenUrl: /v2/oauth/token/
  name: oauth2
  sources:
  - openapi/narmi-public-openapi-original.yml
  type: oauth2
slug: narmi-authentication
source_filename: narmi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/narmi-public-openapi-original.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v2/oauth/authorize/\n    tokenUrl: /v2/oauth/token/\n    scopes: 9\n  sources:\n  - openapi/narmi-public-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/narmi/refs/heads/main/authentication/narmi-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Digital Banking
- Banking
- Payments
- ACH
- Wires
- FedNow
- Cards
- Financial Services
---
