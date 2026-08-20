---
api_key_in: []
api_specs:
- filename: facebook-pages-comments-api-openapi.yml
  format: yaml
  label: Facebook Pages API Comments API
  slug: facebook-pages-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/openapi/facebook-pages-comments-api-openapi.yml
- filename: facebook-pages-conversations-api-openapi.yml
  format: yaml
  label: Facebook Pages API Conversations API
  slug: facebook-pages-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/openapi/facebook-pages-conversations-api-openapi.yml
- filename: facebook-pages-feed-api-openapi.yml
  format: yaml
  label: Facebook Pages API Feed API
  slug: facebook-pages-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/openapi/facebook-pages-feed-api-openapi.yml
- filename: facebook-pages-insights-api-openapi.yml
  format: yaml
  label: Facebook Pages API Insights API
  slug: facebook-pages-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/openapi/facebook-pages-insights-api-openapi.yml
- filename: facebook-pages-me-api-openapi.yml
  format: yaml
  label: Facebook Pages API Me API
  slug: facebook-pages-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/openapi/facebook-pages-me-api-openapi.yml
- filename: facebook-pages-meta-graph-api-pages-api-openapi.yml
  format: yaml
  label: Facebook Pages API Meta Graph API Pages API
  slug: facebook-pages-meta-graph-api-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/openapi/facebook-pages-meta-graph-api-pages-api-openapi.yml
- filename: facebook-pages-photos-api-openapi.yml
  format: yaml
  label: Facebook Pages API Photos API
  slug: facebook-pages-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/openapi/facebook-pages-photos-api-openapi.yml
- filename: facebook-pages-posts-api-openapi.yml
  format: yaml
  label: Facebook Pages API Posts API
  slug: facebook-pages-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/openapi/facebook-pages-posts-api-openapi.yml
- filename: facebook-pages-settings-api-openapi.yml
  format: yaml
  label: Facebook Pages API Settings API
  slug: facebook-pages-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/openapi/facebook-pages-settings-api-openapi.yml
- filename: facebook-pages-subscribed-apps-api-openapi.yml
  format: yaml
  label: Facebook Pages API Subscribed Apps API
  slug: facebook-pages-subscribed-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/openapi/facebook-pages-subscribed-apps-api-openapi.yml
- filename: facebook-pages-tagged-api-openapi.yml
  format: yaml
  label: Facebook Pages API Tagged API
  slug: facebook-pages-tagged-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/openapi/facebook-pages-tagged-api-openapi.yml
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
- Social-Media
- Facebook
- Meta Graph API
- Pages
- Content Publishing
- Social Insights
---
