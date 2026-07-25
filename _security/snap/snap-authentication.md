---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Snap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snap declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Snap
provider_slug: snap
scheme_count: 0
schemes: []
slug: snap-authentication
source_filename: snap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.snap.com/api/marketing-api/Ads-API/authentication\napi: Snapchat Marketing API\nsummary: >-\n  The Snapchat Marketing API uses OAuth 2.0 (authorization code grant with\n  refresh tokens). Access tokens are Bearer tokens presented in the\n  Authorization header and reflect the authorizing user's permissions. Access\n  tokens are short-lived (3600 seconds); refresh tokens are long-lived and used\n  to mint new access tokens on 401 \"token expired\".\nsecurity_schemes:\n  - name: oauth2\n    type: oauth2\n    flow: authorizationCode\n    authorization_endpoint: https://accounts.snapchat.com/login/oauth2/authorize\n    token_endpoint: https://accounts.snapchat.com/login/oauth2/access_token\n    refresh: true\n    token_type: Bearer\n    access_token_ttl_seconds: 3600\n    header: \"Authorization: Bearer {access_token}\"\n    grants:\n      - authorization_code\n      - refresh_token\n    parameters:\n      authorize:\
  \ [client_id, redirect_uri, response_type=code, scope, state]\n      token: [client_id, client_secret, code, grant_type, redirect_uri]\n    scopes:\n      - snapchat-marketing-api\n      - snapchat-offline-conversions-api\n      - snapchat-profile-api\nsnap_kit_login:\n  summary: >-\n    Snap Kit / Login Kit provides \"Login with Snapchat\" built on OAuth 2.0 with\n    OpenID Connect support for identity, returning approved profile fields.\n  docs: https://developers.snap.com/snap-kit/login-kit/Technical-Documentation/OAuth2\n  type: [oauth2, openIdConnect]\nnotes: >-\n  Error on expired token returns HTTP 401 with header\n  `WWW-Authenticate: Bearer error=\"invalid_token\", error_description=\"The access\n  token expired\"`. Many standard OAuth 2.0 client libraries handle the\n  refresh-and-retry pattern automatically.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snap/refs/heads/main/authentication/snap-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Advertising
- Marketing
- Social Media
- Augmented Reality
- Camera
- Authentication
- Identity
- Conversions
- Attribution
- SDKs
---
