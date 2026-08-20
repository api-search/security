---
api_key_in: []
api_specs:
- filename: instagram-comments-api-openapi.yml
  format: yaml
  label: Instagram Comments API
  slug: instagram-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-comments-api-openapi.yml
- filename: instagram-hashtags-api-openapi.yml
  format: yaml
  label: Instagram Hashtags API
  slug: instagram-hashtags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-hashtags-api-openapi.yml
- filename: instagram-insights-api-openapi.yml
  format: yaml
  label: Instagram Insights API
  slug: instagram-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-insights-api-openapi.yml
- filename: instagram-media-api-openapi.yml
  format: yaml
  label: Instagram Media API
  slug: instagram-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-media-api-openapi.yml
- filename: instagram-mentions-api-openapi.yml
  format: yaml
  label: Instagram Mentions API
  slug: instagram-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-mentions-api-openapi.yml
- filename: instagram-publishing-api-openapi.yml
  format: yaml
  label: Instagram Publishing API
  slug: instagram-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-publishing-api-openapi.yml
- filename: instagram-users-api-openapi.yml
  format: yaml
  label: Instagram Users API
  slug: instagram-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Instagram Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Instagram secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Instagram
provider_slug: instagram
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication via Instagram Login or Facebook Login.
  flows:
  - authorizationUrl: https://www.facebook.com/dialog/oauth
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://graph.facebook.com/oauth/access_token
  name: oauth2
  sources:
  - openapi/instagram-graph-api.yaml
  type: oauth2
slug: instagram-authentication
source_filename: instagram-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/instagram-graph-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.facebook.com/dialog/oauth\n    tokenUrl: https://graph.facebook.com/oauth/access_token\n    scopes: 7\n  description: OAuth 2.0 authentication via Instagram Login or Facebook Login.\n  sources:\n  - openapi/instagram-graph-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/authentication/instagram-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Instagram
- Meta
- Photos
- Social-Media
- Videos
- Content Publishing
---
