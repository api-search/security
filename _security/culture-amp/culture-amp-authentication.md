---
api_key_in: []
api_specs:
- filename: spec
  format: yaml
  label: Culture Amp Public API
  slug: culture-amp-public-api
  spec_type: OpenAPI
  url: https://api.cultureamp.com/spec
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Culture Amp Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Culture Amp secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Culture Amp
provider_slug: culture-amp
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: /oauth2/token
  name: Oauth2
  sources:
  - openapi/culture-amp-public-api-openapi.yml
  type: oauth2
slug: culture-amp-authentication
source_filename: culture-amp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/culture-amp-public-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n    scopes: 3\n  sources:\n  - openapi/culture-amp-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culture-amp/refs/heads/main/authentication/culture-amp-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- HR
- Employee Engagement
- Performance Management
- People Analytics
- Surveys
- Human Resources
---
