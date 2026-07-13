---
api_key_in: []
api_specs:
- filename: carnegie-mellon-university-kilthub-figshare.yaml
  format: yaml
  label: KiltHub Repository OAI-PMH (figshare)
  slug: kilthub-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-kilthub-figshare.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Carnegie Mellon University Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Carnegie Mellon University secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Carnegie Mellon University
provider_slug: carnegie-mellon-university
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/carnegie-mellon-university-kilthub-figshare.yaml
  type: oauth2
slug: carnegie-mellon-university-authentication
source_filename: carnegie-mellon-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/carnegie-mellon-university-kilthub-figshare.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/carnegie-mellon-university-kilthub-figshare.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/authentication/carnegie-mellon-university-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- United States
- Research
- Epidemiology
- Open Data
- Library
- Institutional Repository
---
