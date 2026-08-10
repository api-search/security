---
api_key_in: []
api_specs:
- filename: sketchfab-download-api-openapi.yml
  format: yaml
  label: Sketchfab Download API
  slug: sketchfab-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-download-api-openapi.yml
- filename: sketchfab-oembed-api-openapi.yml
  format: yaml
  label: Sketchfab oEmbed API
  slug: sketchfab-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-oembed-api-openapi.yml
- filename: sketchfab-oauth-api-openapi.yml
  format: yaml
  label: Sketchfab OAuth 2.0 API
  slug: sketchfab-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-oauth-api-openapi.yml
- filename: sketchfab-bookmarks-api-openapi.yml
  format: yaml
  label: Sketchfab Bookmarks API
  slug: sketchfab-bookmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-bookmarks-api-openapi.yml
- filename: sketchfab-categories-api-openapi.yml
  format: yaml
  label: Sketchfab Categories API
  slug: sketchfab-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-categories-api-openapi.yml
- filename: sketchfab-collections-api-openapi.yml
  format: yaml
  label: Sketchfab Collections API
  slug: sketchfab-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-collections-api-openapi.yml
- filename: sketchfab-comments-api-openapi.yml
  format: yaml
  label: Sketchfab Comments API
  slug: sketchfab-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-comments-api-openapi.yml
- filename: sketchfab-likes-api-openapi.yml
  format: yaml
  label: Sketchfab Likes API
  slug: sketchfab-likes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-likes-api-openapi.yml
- filename: sketchfab-models-api-openapi.yml
  format: yaml
  label: Sketchfab Models API
  slug: sketchfab-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-models-api-openapi.yml
- filename: sketchfab-orgs-api-openapi.yml
  format: yaml
  label: Sketchfab Orgs API
  slug: sketchfab-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-orgs-api-openapi.yml
- filename: sketchfab-search-api-openapi.yml
  format: yaml
  label: Sketchfab Search API
  slug: sketchfab-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-search-api-openapi.yml
- filename: sketchfab-tags-api-openapi.yml
  format: yaml
  label: Sketchfab Tags API
  slug: sketchfab-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-tags-api-openapi.yml
- filename: sketchfab-users-api-openapi.yml
  format: yaml
  label: Sketchfab Users API
  slug: sketchfab-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sketchfab Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Sketchfab secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Sketchfab
provider_slug: sketchfab
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://sketchfab.com/oauth2/authorize/
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://sketchfab.com/oauth2/token/
  name: OAuth2
  sources:
  - openapi/sketchfab-download-api-openapi.yml
  type: oauth2
slug: sketchfab-authentication
source_filename: sketchfab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sketchfab-download-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sketchfab.com/oauth2/authorize/\n    tokenUrl: https://sketchfab.com/oauth2/token/\n    scopes: 1\n  sources:\n  - openapi/sketchfab-download-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/authentication/sketchfab-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- 3D
- Models
- Marketplace
- Viewer
- WebGL
- glTF
- AR
- VR
- Creative
- Epic Games
---
