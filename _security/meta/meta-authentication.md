---
api_key_in: []
api_specs:
- filename: meta-openapi.yml
  format: yaml
  label: Facebook Graph API - User
  slug: facebook-graph-api-user
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meta/refs/heads/main/openapi/meta-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Meta Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Meta secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Meta
provider_slug: meta
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth
    flow: implicit
    scopes: 1
  name: userAccessToken
  sources:
  - openapi/meta-openapi.yml
  type: oauth2
slug: meta-authentication
source_filename: meta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/meta-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: userAccessToken\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth\n    scopes: 1\n  sources:\n  - openapi/meta-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meta/refs/heads/main/authentication/meta-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advertising
- Analytics
- Artificial Intelligence
- Messaging
- Social
- Social Media
- Virtual Reality
---
