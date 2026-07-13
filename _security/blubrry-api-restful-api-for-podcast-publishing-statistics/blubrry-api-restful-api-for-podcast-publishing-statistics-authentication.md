---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Blubrry Api Restful Api For Podcast Publishing Statistics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Blubrry API secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Blubrry API
provider_slug: blubrry-api-restful-api-for-podcast-publishing-statistics
scheme_count: 1
schemes:
- description: 'OAuth 2.0 Bearer token. Contact Blubrry to receive a client_id and

    secret. Tokens expire after one hour; refresh tokens do not expire.'
  flows:
  - authorizationUrl: https://api.blubrry.com/oauth2/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.blubrry.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-openapi.yml
  type: oauth2
slug: blubrry-api-restful-api-for-podcast-publishing-statistics-authentication
source_filename: blubrry-api-restful-api-for-podcast-publishing-statistics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.blubrry.com/oauth2/authorize\n    tokenUrl: https://api.blubrry.com/oauth2/token\n    scopes: 0\n  description: |-\n    OAuth 2.0 Bearer token. Contact Blubrry to receive a client_id and\n    secret. Tokens expire after one hour; refresh tokens do not expire.\n  sources:\n  - openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blubrry-api-restful-api-for-podcast-publishing-statistics/refs/heads/main/authentication/blubrry-api-restful-api-for-podcast-publishing-statistics-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Podcasting
- Audio
- Media
- Publishing
- Statistics
---
