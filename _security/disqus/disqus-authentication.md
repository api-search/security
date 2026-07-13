---
api_key_in:
- query
api_specs:
- filename: disqus-openapi.yml
  format: yaml
  label: Disqus Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disqus/refs/heads/main/openapi/disqus-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Disqus Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Disqus secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Disqus
provider_slug: disqus
scheme_count: 2
schemes:
- in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/disqus-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://disqus.com/api/oauth/2.0/authorize/
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://disqus.com/api/oauth/2.0/access_token/
  name: oauth2
  sources:
  - openapi/disqus-openapi.yml
  type: oauth2
slug: disqus-authentication
source_filename: disqus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/disqus-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/disqus-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://disqus.com/api/oauth/2.0/authorize/\n    tokenUrl: https://disqus.com/api/oauth/2.0/access_token/\n    scopes: 3\n  sources:\n  - openapi/disqus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/disqus/refs/heads/main/authentication/disqus-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Comments
- Community
- Discussions
- Publishing
- Audience Engagement
- Social
---
