---
api_key_in: []
api_specs:
- filename: podbean-analytics-api-openapi.yml
  format: yaml
  label: Podbean Analytics API
  slug: podbean-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-analytics-api-openapi.yml
- filename: podbean-authentication-api-openapi.yml
  format: yaml
  label: Podbean Authentication API
  slug: podbean-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-authentication-api-openapi.yml
- filename: podbean-episode-api-openapi.yml
  format: yaml
  label: Podbean Episode API
  slug: podbean-episode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-episode-api-openapi.yml
- filename: podbean-file-upload-api-openapi.yml
  format: yaml
  label: Podbean File Upload API
  slug: podbean-file-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-file-upload-api-openapi.yml
- filename: podbean-oembed-api-openapi.yml
  format: yaml
  label: Podbean oEmbed API
  slug: podbean-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-oembed-api-openapi.yml
- filename: podbean-podcast-api-openapi.yml
  format: yaml
  label: Podbean Podcast API
  slug: podbean-podcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-podcast-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Podbean Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Podbean secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Podbean
provider_slug: podbean
scheme_count: 1
schemes:
- description: OAuth 2.0. Register an app at developers.podbean.com to obtain a Client ID and Secret.
  flows:
  - authorizationUrl: https://api.podbean.com/v1/dialog/oauth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api.podbean.com/v1/oauth/token
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.podbean.com/v1/oauth/token
  name: oauth2
  sources:
  - openapi/podbean-openapi.yml
  type: oauth2
slug: podbean-authentication
source_filename: podbean-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/podbean-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.podbean.com/v1/dialog/oauth\n    tokenUrl: https://api.podbean.com/v1/oauth/token\n    scopes: 3\n  - flow: clientCredentials\n    tokenUrl: https://api.podbean.com/v1/oauth/token\n    scopes: 2\n  description: OAuth 2.0. Register an app at developers.podbean.com to obtain a Client ID and\n    Secret.\n  sources:\n  - openapi/podbean-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/authentication/podbean-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Podcasting
- Podcast Hosting
- Media
- Audio
- Episodes
- Analytics
- Monetization
---
