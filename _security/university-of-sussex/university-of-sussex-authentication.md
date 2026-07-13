---
api_key_in: []
api_specs:
- filename: university-of-sussex-figshare-repository.yaml
  format: yaml
  label: University of Sussex Research Repository (Figshare)
  slug: figshare-repository
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/openapi/university-of-sussex-figshare-repository.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: University Of Sussex Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: University of Sussex secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: University of Sussex
provider_slug: university-of-sussex
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/university-of-sussex-figshare-repository.yaml
  type: oauth2
slug: university-of-sussex-authentication
source_filename: university-of-sussex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-sussex-figshare-repository.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/university-of-sussex-figshare-repository.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/authentication/university-of-sussex-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- United Kingdom
---
