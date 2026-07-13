---
api_key_in: []
api_specs:
- filename: tidal-catalog-api-openapi.yml
  format: yaml
  label: TIDAL Catalog API
  slug: tidal-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-catalog-api-openapi.yml
- filename: tidal-search-api-openapi.yml
  format: yaml
  label: TIDAL Search API
  slug: tidal-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-search-api-openapi.yml
- filename: tidal-playlists-api-openapi.yml
  format: yaml
  label: TIDAL Playlists API
  slug: tidal-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-playlists-api-openapi.yml
- filename: tidal-users-api-openapi.yml
  format: yaml
  label: TIDAL Users API
  slug: tidal-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-users-api-openapi.yml
- filename: tidal-user-collections-api-openapi.yml
  format: yaml
  label: TIDAL User Collections API
  slug: tidal-user-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-user-collections-api-openapi.yml
- filename: tidal-recommendations-api-openapi.yml
  format: yaml
  label: TIDAL Recommendations API
  slug: tidal-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-recommendations-api-openapi.yml
- filename: tidal-playback-api-openapi.yml
  format: yaml
  label: TIDAL Playback API
  slug: tidal-playback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-playback-api-openapi.yml
- filename: tidal-social-api-openapi.yml
  format: yaml
  label: TIDAL Social API
  slug: tidal-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-social-api-openapi.yml
- filename: tidal-commerce-api-openapi.yml
  format: yaml
  label: TIDAL Commerce API
  slug: tidal-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-commerce-api-openapi.yml
- filename: tidal-claims-api-openapi.yml
  format: yaml
  label: TIDAL Claims API
  slug: tidal-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-claims-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tidal Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: TIDAL secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: TIDAL
provider_slug: tidal
scheme_count: 2
schemes:
- description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code
  flows:
  - authorizationUrl: https://login.tidal.com/authorize
    flow: authorizationCode
    scopes: 12
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Authorization_Code_PKCE
  sources:
  - openapi/tidal-catalog-api-openapi.yml
  - openapi/tidal-claims-api-openapi.yml
  - openapi/tidal-commerce-api-openapi.yml
  - openapi/tidal-playback-api-openapi.yml
  - openapi/tidal-playlists-api-openapi.yml
  - openapi/tidal-recommendations-api-openapi.yml
  - openapi/tidal-search-api-openapi.yml
  - openapi/tidal-social-api-openapi.yml
  - openapi/tidal-user-collections-api-openapi.yml
  - openapi/tidal-users-api-openapi.yml
  type: oauth2
- description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Client_Credentials
  sources:
  - openapi/tidal-catalog-api-openapi.yml
  - openapi/tidal-claims-api-openapi.yml
  - openapi/tidal-commerce-api-openapi.yml
  - openapi/tidal-playback-api-openapi.yml
  - openapi/tidal-playlists-api-openapi.yml
  - openapi/tidal-recommendations-api-openapi.yml
  - openapi/tidal-search-api-openapi.yml
  - openapi/tidal-social-api-openapi.yml
  - openapi/tidal-user-collections-api-openapi.yml
  - openapi/tidal-users-api-openapi.yml
  type: oauth2
slug: tidal-authentication
source_filename: tidal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tidal-catalog-api-openapi.yml, openapi/tidal-claims-api-openapi.yml, openapi/tidal-commerce-api-openapi.yml,\n  openapi/tidal-playback-api-openapi.yml, openapi/tidal-playlists-api-openapi.yml, openapi/tidal-recommendations-api-openapi.yml,\n  openapi/tidal-search-api-openapi.yml, openapi/tidal-social-api-openapi.yml, openapi/tidal-user-collections-api-openapi.yml,\n  openapi/tidal-users-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: Authorization_Code_PKCE\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.tidal.com/authorize\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n    scopes: 12\n  description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n  - openapi/tidal-claims-api-openapi.yml\n\
  \  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n  - openapi/tidal-recommendations-api-openapi.yml\n  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n  - openapi/tidal-user-collections-api-openapi.yml\n  - openapi/tidal-users-api-openapi.yml\n- name: Client_Credentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n    scopes: 0\n  description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n  - openapi/tidal-claims-api-openapi.yml\n  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n  - openapi/tidal-recommendations-api-openapi.yml\n  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n  - openapi/tidal-user-collections-api-openapi.yml\n\
  \  - openapi/tidal-users-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/authentication/tidal-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Music
- Streaming
- Hi-Fi
- HiRes Lossless
- Audio
- Block
- Square
---
