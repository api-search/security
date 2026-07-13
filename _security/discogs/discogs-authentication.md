---
api_key_in:
- header
api_specs:
- filename: discogs-openapi-original.yml
  format: yaml
  label: Discogs API
  slug: discogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discogs/refs/heads/main/openapi/discogs-openapi-original.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Discogs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Discogs secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Discogs
provider_slug: discogs
scheme_count: 2
schemes:
- description: 'Discogs personal access token in header: ''Discogs token={token}''.'
  in: header
  name: DiscogsToken
  parameter: Authorization
  sources:
  - openapi/discogs-openapi-original.yml
  type: apiKey
- description: OAuth 1.0a flow modeled as OAuth2 for tooling. Required for write actions on behalf of other users.
  flows:
  - authorizationUrl: https://discogs.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.discogs.com/oauth/access_token
  name: OAuth1
  sources:
  - openapi/discogs-openapi-original.yml
  type: oauth2
slug: discogs-authentication
source_filename: discogs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/discogs-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: DiscogsToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Discogs personal access token in header: ''Discogs token={token}''.'\n  sources:\n  - openapi/discogs-openapi-original.yml\n- name: OAuth1\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://discogs.com/oauth/authorize\n    tokenUrl: https://api.discogs.com/oauth/access_token\n    scopes: 2\n  description: OAuth 1.0a flow modeled as OAuth2 for tooling. Required for write actions on\n    behalf of other users.\n  sources:\n  - openapi/discogs-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discogs/refs/heads/main/authentication/discogs-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Music
- Marketplace
- Catalog
- Community
- Vinyl
- Public APIs
---
