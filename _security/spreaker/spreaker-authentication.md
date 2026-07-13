---
api_key_in: []
api_specs:
- filename: spreaker-openapi.yml
  format: yaml
  label: Spreaker Users API
  slug: spreaker-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/openapi/spreaker-openapi.yml
- filename: spreaker-openapi.yml
  format: yaml
  label: Spreaker Shows API
  slug: spreaker-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/openapi/spreaker-openapi.yml
- filename: spreaker-openapi.yml
  format: yaml
  label: Spreaker Episodes API
  slug: spreaker-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/openapi/spreaker-openapi.yml
- filename: spreaker-openapi.yml
  format: yaml
  label: Spreaker Statistics API
  slug: spreaker-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/openapi/spreaker-openapi.yml
- filename: spreaker-openapi.yml
  format: yaml
  label: Spreaker Search and Discovery API
  slug: spreaker-search-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/openapi/spreaker-openapi.yml
- filename: spreaker-openapi.yml
  format: yaml
  label: Spreaker Advertising Campaigns API
  slug: spreaker-advertising-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/openapi/spreaker-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Spreaker Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Spreaker secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Spreaker
provider_slug: spreaker
scheme_count: 1
schemes:
- description: OAuth2. Authorize at https://www.spreaker.com/oauth2/authorize and exchange or refresh tokens at https://api.spreaker.com/oauth2/token. Access tokens are sent as a Bearer token in the Authorization header.
  flows:
  - authorizationUrl: https://www.spreaker.com/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.spreaker.com/oauth2/token
  name: oauth2
  sources:
  - openapi/spreaker-openapi.yml
  type: oauth2
slug: spreaker-authentication
source_filename: spreaker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spreaker-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.spreaker.com/oauth2/authorize\n    tokenUrl: https://api.spreaker.com/oauth2/token\n    scopes: 1\n  description: OAuth2. Authorize at https://www.spreaker.com/oauth2/authorize and exchange or\n    refresh tokens at https://api.spreaker.com/oauth2/token. Access tokens are sent as a Bearer\n    token in the Authorization header.\n  sources:\n  - openapi/spreaker-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/authentication/spreaker-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Podcasting
- Podcast Hosting
- Audio
- Media
- Monetization
- Analytics
---
