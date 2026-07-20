---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ellipsis Drive Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ellipsis Drive secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ellipsis Drive
provider_slug: ellipsis-drive
scheme_count: 2
schemes:
- description: 'Personal or OAuth-issued access token passed as `Authorization: Bearer <token>`. Personal access tokens are managed at Account > Access tokens.'
  docs: https://docs.ellipsis-drive.com/developers/api-v3/account/access-tokens
  name: bearerAuth
  scheme: bearer
  sources:
  - docs
  type: http
- description: OAuth2 authorization-code flow (PKCE supported) for delegated third-party access.
  docs: https://docs.ellipsis-drive.com/developers/api-v3/oauth/authorization
  flows:
  - authorizationUrl: https://api.ellipsis-drive.com/v3/oauth/authorize
    flow: authorizationCode
    scopes:
      projects: Allows the use of all API calls except those in /settings/account (default and currently the only scope).
  name: oauth2
  sources:
  - docs
  type: oauth2
slug: ellipsis-drive-authentication
source_filename: ellipsis-drive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.ellipsis-drive.com/developers/api-v3\ndocs: https://docs.ellipsis-drive.com/developers/api-v3/oauth/authorization\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    Requests authenticate with a Bearer access token in the Authorization header. Tokens can be\n    created and managed under the account (personal access tokens) or obtained via the OAuth2\n    authorization-code flow (PKCE supported) for third-party integrations.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Personal or OAuth-issued access token passed as `Authorization: Bearer <token>`. Personal\n    access tokens are managed at Account > Access tokens.\n  docs: https://docs.ellipsis-drive.com/developers/api-v3/account/access-tokens\n  sources: [docs]\n- name: oauth2\n  type: oauth2\n  description: OAuth2 authorization-code flow (PKCE supported) for\
  \ delegated third-party access.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.ellipsis-drive.com/v3/oauth/authorize\n    scopes:\n      projects: Allows the use of all API calls except those in /settings/account (default and currently the only scope).\n  docs: https://docs.ellipsis-drive.com/developers/api-v3/oauth/authorization\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ellipsis-drive/refs/heads/main/authentication/ellipsis-drive-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Geospatial
- Spatial Data
- GIS
- Mapping
- Data Management
- Raster
- Vector
- OGC
- Cloud Storage
- Remote Sensing
---
