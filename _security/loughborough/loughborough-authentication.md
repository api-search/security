---
api_key_in: []
api_specs:
- filename: loughborough-research-repository-rest.yaml
  format: yaml
  label: Loughborough Research Repository (figshare REST API)
  slug: research-repository-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-research-repository-rest.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Loughborough Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Loughborough University secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Loughborough University
provider_slug: loughborough
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/loughborough-research-repository-rest.yaml
  type: oauth2
slug: loughborough-authentication
source_filename: loughborough-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/loughborough-research-repository-rest.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/loughborough-research-repository-rest.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/authentication/loughborough-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- United Kingdom
- Research Data
- Open Access
- Repository
- Identity
---
