---
api_key_in: []
api_specs:
- filename: facebook-pages-openapi.yml
  format: yaml
  label: Meta Graph API - Pages
  slug: graph-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/openapi/facebook-pages-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Facebook Pages Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Facebook Pages API secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Facebook Pages API
provider_slug: facebook-pages
scheme_count: 1
schemes:
- description: 'OAuth 2.0 Page access token. Granted scopes determine which

    endpoints can be called. Send as a Bearer token or as the

    access_token query parameter.'
  flows:
  - authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://graph.facebook.com/v22.0/oauth/access_token
  name: PageAccessToken
  sources:
  - openapi/facebook-pages-openapi.yml
  type: oauth2
slug: facebook-pages-authentication
source_filename: facebook-pages-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/facebook-pages-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: PageAccessToken\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth\n    tokenUrl: https://graph.facebook.com/v22.0/oauth/access_token\n    scopes: 7\n  description: |-\n    OAuth 2.0 Page access token. Granted scopes determine which\n    endpoints can be called. Send as a Bearer token or as the\n    access_token query parameter.\n  sources:\n  - openapi/facebook-pages-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/authentication/facebook-pages-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Social Media
- Facebook
- Meta Graph API
- Pages
- Content Publishing
- Social Insights
---
