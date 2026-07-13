---
api_key_in: []
api_specs:
- filename: university-of-auckland-figshare-rest.yaml
  format: yaml
  label: University of Auckland Figshare Research Repository API
  slug: figshare-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-figshare-rest.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: University Of Auckland Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: University of Auckland secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: University of Auckland
provider_slug: university-of-auckland
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/university-of-auckland-figshare-rest.yaml
  type: oauth2
slug: university-of-auckland-authentication
source_filename: university-of-auckland-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-auckland-figshare-rest.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/university-of-auckland-figshare-rest.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/authentication/university-of-auckland-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- New Zealand
---
