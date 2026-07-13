---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Canva Connect API
  slug: canva-connect-api
  spec_type: OpenAPI
  url: https://www.canva.com/developers/docs/connect-api/openapi/
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Canva Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Canva secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Canva
provider_slug: canva
scheme_count: 1
schemes:
- description: Canva uses OAuth 2.0 with authorization code flow. Access tokens must be included in the Authorization header as a Bearer token.
  flows:
  - authorizationUrl: https://www.canva.com/api/oauth/authorize
    flow: authorizationCode
    scopes: 11
    tokenUrl: https://api.canva.com/rest/v1/oauth/token
  name: oauth2
  sources:
  - openapi/canva-connect-api-openapi.yml
  type: oauth2
slug: canva-authentication
source_filename: canva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/canva-connect-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.canva.com/api/oauth/authorize\n    tokenUrl: https://api.canva.com/rest/v1/oauth/token\n    scopes: 11\n  description: Canva uses OAuth 2.0 with authorization code flow. Access tokens must be included\n    in the Authorization header as a Bearer token.\n  sources:\n  - openapi/canva-connect-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/authentication/canva-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Apps
- Automation
- Brand Management
- Collaboration
- Design
- Graphics
- Marketing
- Print
- Templates
- Visual Content
---
