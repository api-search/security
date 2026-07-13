---
api_key_in: []
api_specs:
- filename: aweber-openapi.yml
  format: yaml
  label: AWeber REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Aweber Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AWeber secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AWeber
provider_slug: aweber
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://auth.aweber.com/oauth2/authorize
    flow: authorizationCode
    scopes: 9
    tokenUrl: https://auth.aweber.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/aweber-openapi.yml
  type: oauth2
slug: aweber-authentication
source_filename: aweber-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aweber-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.aweber.com/oauth2/authorize\n    tokenUrl: https://auth.aweber.com/oauth2/token\n    scopes: 9\n  sources:\n  - openapi/aweber-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/authentication/aweber-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Email Marketing
- Marketing Automation
- Email
- Newsletters
- Subscribers
- Campaigns
- Landing Pages
---
