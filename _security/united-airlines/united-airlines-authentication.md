---
api_key_in: []
api_specs:
- filename: united-airlines-ndc-openapi.yml
  format: yaml
  label: United Airlines NDC API
  slug: united-airlines-ndc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-airlines/main/openapi/united-airlines-ndc-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: United Airlines Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: United Airlines secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: United Airlines
provider_slug: united-airlines
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.united.com/v1/oauth/token
  name: OAuth2
  sources:
  - openapi/united-airlines-ndc-openapi.yml
  type: oauth2
slug: united-airlines-authentication
source_filename: united-airlines-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/united-airlines-ndc-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.united.com/v1/oauth/token\n    scopes: 2\n  sources:\n  - openapi/united-airlines-ndc-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-airlines/refs/heads/main/authentication/united-airlines-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Airlines
- Travel
- Flight Booking
- NDC
- Loyalty
- Fortune 100
---
