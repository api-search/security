---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Livelike Authentication
name_suffix: Authentication
oauth_flows: []
overview: LiveLike secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LiveLike
provider_slug: livelike
scheme_count: 2
schemes:
- description: All requests are authenticated with OAuth 2.0 Bearer authentication via the Authorization header. Access Tokens are obtained by creating a Profile through the API/SDKs or from the Producer Suite.
  format: Bearer {access-token}
  header: Authorization
  name: OAuth2 Bearer
  scheme: bearer
  token_scopes:
  - description: Scoped to a single profile. Used to interact with widgets and participate in chat on behalf of an end user.
    name: Profile Access Token
    scope: profile
  - description: Scoped to an Application and associated with a Producer. Broader permissions; used for server-to-server automations such as creating programs and publishing widgets. Also called API / Producer Access Token.
    name: Admin Access Token
    scope: application
  type: oauth2
- description: 'Site-wide / organization-wide administrative token for tasks such as creating and managing applications. Obtained from the My Account page in the LiveLike Producer CMS. Sent as `Authorization: Token {token}`.'
  format: Token {personal-api-token}
  in: header
  name: Personal API Token
  parameter_name: Authorization
  type: apiKey
slug: livelike-authentication
source_filename: livelike-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.livelike.com/reference/authentication\ndocs: https://docs.livelike.com/reference/authentication\nsummary:\n  types: [oauth2, http]\n  transport: Authorization HTTP header\n  token_types: [Profile Access Token, Admin Access Token, Personal API Token]\nschemes:\n- name: OAuth2 Bearer\n  type: oauth2\n  scheme: bearer\n  header: Authorization\n  format: \"Bearer {access-token}\"\n  description: >-\n    All requests are authenticated with OAuth 2.0 Bearer authentication via the\n    Authorization header. Access Tokens are obtained by creating a Profile\n    through the API/SDKs or from the Producer Suite.\n  token_scopes:\n  - name: Profile Access Token\n    scope: profile\n    description: >-\n      Scoped to a single profile. Used to interact with widgets and participate\n      in chat on behalf of an end user.\n  - name: Admin Access Token\n    scope: application\n    description: >-\n      Scoped to an Application\
  \ and associated with a Producer. Broader\n      permissions; used for server-to-server automations such as creating\n      programs and publishing widgets. Also called API / Producer Access Token.\n- name: Personal API Token\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  format: \"Token {personal-api-token}\"\n  description: >-\n    Site-wide / organization-wide administrative token for tasks such as\n    creating and managing applications. Obtained from the My Account page in the\n    LiveLike Producer CMS. Sent as `Authorization: Token {token}`.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/livelike/refs/heads/main/authentication/livelike-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Fan Engagement
- Live Streaming
- Interactive Video
- Chat
- Gamification
- Widgets
- Sports
- Media
---
