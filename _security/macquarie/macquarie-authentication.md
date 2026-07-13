---
api_key_in: []
api_specs:
- filename: macquarie-rdr-figshare.yaml
  format: yaml
  label: Macquarie University Research Data Repository (Figshare API)
  slug: rdr-figshare
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/openapi/macquarie-rdr-figshare.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Macquarie Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Macquarie University secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Macquarie University
provider_slug: macquarie
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/macquarie-rdr-figshare.yaml
  type: oauth2
slug: macquarie-authentication
source_filename: macquarie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/macquarie-rdr-figshare.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/macquarie-rdr-figshare.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/authentication/macquarie-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Research Data
- Library
- Australia
---
