---
api_key_in: []
api_specs:
- filename: kadence-public-api-openapi.yml
  format: yaml
  label: Kadence Public API
  slug: kadence-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-public-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Kadence Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Kadence secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Kadence
provider_slug: kadence
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials Grant
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.onkadence.co/oauth2/token
  name: oauth
  sources:
  - openapi/kadence-public-api-openapi.yml
  type: oauth2
slug: kadence-authentication
source_filename: kadence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/kadence-public-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.onkadence.co/oauth2/token\n    scopes: 1\n  description: OAuth 2.0 client credentials Grant\n  sources:\n  - openapi/kadence-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/authentication/kadence-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Workplace
- Hybrid Work
- Desk Booking
- Room Booking
- Space Management
- Visitor Management
- Workplace Analytics
- Facilities
- OAuth
---
