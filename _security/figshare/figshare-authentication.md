---
api_key_in: []
api_specs:
- filename: swagger.json
  format: json
  label: Figshare API
  slug: figshare-api
  spec_type: OpenAPI
  url: https://docs.figshare.com/swagger.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Figshare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Figshare secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Figshare
provider_slug: figshare
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/figshare-api-openapi.yml
  type: oauth2
slug: figshare-authentication
source_filename: figshare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/figshare-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/figshare-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figshare/refs/heads/main/authentication/figshare-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Research Data
- Data Repository
- Open Science
- DOI
- Datasets
- Academic
- File Storage
- Open Access
---
