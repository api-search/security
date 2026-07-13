---
api_key_in: []
api_specs:
- filename: cms-energy-openapi.yml
  format: yaml
  label: Consumers Energy Green Button Connect My Data API
  slug: consumers-green-button-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cms Energy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CMS Energy secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CMS Energy
provider_slug: cms-energy
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://utilityapi.com/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://utilityapi.com/api/v2/oauth/token
  name: oauth2
  sources:
  - openapi/cms-energy-openapi.yml
  type: oauth2
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cms-energy-openapi.yml
  type: http
slug: cms-energy-authentication
source_filename: cms-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cms-energy-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://utilityapi.com/authorize\n    tokenUrl: https://utilityapi.com/api/v2/oauth/token\n    scopes: 1\n  sources:\n  - openapi/cms-energy-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cms-energy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/authentication/cms-energy-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Electric
- Energy
- Green Button
- Michigan
- Natural Gas
- Utility
- Fortune 500
---
