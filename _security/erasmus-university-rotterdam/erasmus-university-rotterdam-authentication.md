---
api_key_in: []
api_specs:
- filename: erasmus-university-rotterdam-figshare-data.yaml
  format: yaml
  label: EUR Research Data Repository (Figshare API)
  slug: figshare-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/openapi/erasmus-university-rotterdam-figshare-data.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Erasmus University Rotterdam Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Erasmus University Rotterdam secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Erasmus University Rotterdam
provider_slug: erasmus-university-rotterdam
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/erasmus-university-rotterdam-figshare-data.yaml
  type: oauth2
slug: erasmus-university-rotterdam-authentication
source_filename: erasmus-university-rotterdam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/erasmus-university-rotterdam-figshare-data.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/erasmus-university-rotterdam-figshare-data.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/authentication/erasmus-university-rotterdam-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Repository
- OAI-PMH
- Netherlands
---
