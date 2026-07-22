---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Unruly Studios Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unruly Studios declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Unruly Studios
provider_slug: unruly-studios
scheme_count: 3
schemes:
- description: GitLab OAuth 2.0 authorization server on the Gamelocker host.
  flows:
    authorization_code:
      authorization_url: https://gamelocker.unruly-studios.com/oauth/authorize
      refresh_url: https://gamelocker.unruly-studios.com/oauth/token
      token_url: https://gamelocker.unruly-studios.com/oauth/token
    client_credentials:
      token_url: https://gamelocker.unruly-studios.com/oauth/token
    password:
      note: The Resource Owner Password Credentials grant is enabled on this instance and is what UnrulyGamelocker.js uses today.
      token_url: https://gamelocker.unruly-studios.com/oauth/token
  grant_types:
  - authorization_code
  - implicit
  - password
  - client_credentials
  - refresh_token
  id: gamelocker_oauth2
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- description: GitLab OpenID Connect provider on the Gamelocker host.
  id: gamelocker_oidc
  id_token_signing_alg: RS256
  issuer: https://gamelocker.unruly-studios.com
  jwks_uri: https://gamelocker.unruly-studios.com/oauth/discovery/keys
  openid_configuration: https://gamelocker.unruly-studios.com/.well-known/openid-configuration
  type: openIdConnect
  userinfo_endpoint: https://gamelocker.unruly-studios.com/oauth/userinfo
- description: GitLab personal/OAuth access token passed as an access_token query parameter (or Authorization bearer header) on /api/v4 requests.
  id: gamelocker_access_token
  in: query
  name: access_token
  type: apiKey
slug: unruly-studios-authentication
source_filename: unruly-studios-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://gamelocker.unruly-studios.com/.well-known/openid-configuration\nnotes: >-\n  Unruly's \"Gamelocker\" project-storage backend (gamelocker.unruly-studios.com)\n  is a self-hosted GitLab instance and exposes GitLab's standard OAuth 2.0 /\n  OpenID Connect authorization server. The client library used by the Unruly\n  Splats app (UnrulyGamelocker.js) authenticates against /oauth/token and calls\n  the GitLab REST API at /api/v4 with a bearer/query access_token. These are\n  GitLab-native auth mechanisms, not a bespoke Unruly auth scheme.\nschemes:\n- id: gamelocker_oauth2\n  type: oauth2\n  description: GitLab OAuth 2.0 authorization server on the Gamelocker host.\n  flows:\n    authorization_code:\n      authorization_url: https://gamelocker.unruly-studios.com/oauth/authorize\n      token_url: https://gamelocker.unruly-studios.com/oauth/token\n      refresh_url: https://gamelocker.unruly-studios.com/oauth/token\n    client_credentials:\n\
  \      token_url: https://gamelocker.unruly-studios.com/oauth/token\n    password:\n      token_url: https://gamelocker.unruly-studios.com/oauth/token\n      note: >-\n        The Resource Owner Password Credentials grant is enabled on this\n        instance and is what UnrulyGamelocker.js uses today.\n  grant_types:\n  - authorization_code\n  - implicit\n  - password\n  - client_credentials\n  - refresh_token\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n- id: gamelocker_oidc\n  type: openIdConnect\n  description: GitLab OpenID Connect provider on the Gamelocker host.\n  openid_configuration: https://gamelocker.unruly-studios.com/.well-known/openid-configuration\n  issuer: https://gamelocker.unruly-studios.com\n  jwks_uri: https://gamelocker.unruly-studios.com/oauth/discovery/keys\n  userinfo_endpoint: https://gamelocker.unruly-studios.com/oauth/userinfo\n  id_token_signing_alg: RS256\n- id: gamelocker_access_token\n  type: apiKey\n  in: query\n  name:\
  \ access_token\n  description: >-\n    GitLab personal/OAuth access token passed as an access_token query\n    parameter (or Authorization bearer header) on /api/v4 requests.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unruly-studios/refs/heads/main/authentication/unruly-studios-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Education
- STEM
- EdTech
- Coding
- Kids
- Learning
- Hardware
---
