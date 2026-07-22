---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Playerdata Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- authorizationCodePKCE
- clientCredentials
overview: PlayerData secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, authorizationCodePKCE, and clientCredentials flow(s).
provider_name: PlayerData
provider_slug: playerdata
scheme_count: 3
schemes:
- authorizationUrl: https://app.playerdata.co.uk/oauth/authorize
  flow: authorizationCode
  name: OAuth2AuthorizationCode
  sources:
  - https://github.com/PlayerData/playerdatapy/blob/main/docs/auth.md
  tokenUrl: https://app.playerdata.co.uk/oauth/token
  type: oauth2
  use_case: Confidential clients with a secret (user-based access)
- authorizationUrl: https://app.playerdata.co.uk/oauth/authorize
  flow: authorizationCode
  name: OAuth2AuthorizationCodePKCE
  pkce: true
  sources:
  - https://github.com/PlayerData/playerdatapy/blob/main/docs/auth.md
  tokenUrl: https://app.playerdata.co.uk/oauth/token
  type: oauth2
  use_case: Public clients with no secret (user-based access)
- flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - https://github.com/PlayerData/playerdatapy/blob/main/docs/auth.md
  tokenUrl: https://app.playerdata.co.uk/oauth/token
  type: oauth2
  use_case: Backend-to-backend, organisation-level access
slug: playerdata-authentication
source_filename: playerdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/PlayerData/playerdatapy/blob/main/docs/auth.md\ndocs: https://github.com/PlayerData/playerdatapy/blob/main/docs/auth.md\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, authorizationCodePKCE, clientCredentials]\n  token_type: Bearer\n  access_token_ttl_seconds: 7200\n  refresh_tokens: true    # authorization code grant only; client credentials re-runs the flow\nnotes: >-\n  The PlayerData API is a GraphQL API secured with OAuth 2.0. Authorisation Code\n  Grant provides user-based access (read + write) mirroring what the user sees in\n  the PlayerData app, with data access governed by club-staff membership. Client\n  Credentials Grant provides server-to-server, organisation-level access for\n  service accounts granted org access. There is no documented OAuth scope surface;\n  authorization is governed by club-staff membership and org-level grants rather\n  than scopes. Credentials are issued\
  \ on request via support@playerdata.com.\nschemes:\n  - name: OAuth2AuthorizationCode\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://app.playerdata.co.uk/oauth/authorize\n    tokenUrl: https://app.playerdata.co.uk/oauth/token\n    use_case: Confidential clients with a secret (user-based access)\n    sources: [https://github.com/PlayerData/playerdatapy/blob/main/docs/auth.md]\n  - name: OAuth2AuthorizationCodePKCE\n    type: oauth2\n    flow: authorizationCode\n    pkce: true\n    authorizationUrl: https://app.playerdata.co.uk/oauth/authorize\n    tokenUrl: https://app.playerdata.co.uk/oauth/token\n    use_case: Public clients with no secret (user-based access)\n    sources: [https://github.com/PlayerData/playerdatapy/blob/main/docs/auth.md]\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://app.playerdata.co.uk/oauth/token\n    use_case: Backend-to-backend, organisation-level access\n    sources: [https://github.com/PlayerData/playerdatapy/blob/main/docs/auth.md]\n\
  endpoints:\n  graphql: https://app.playerdata.co.uk/api/graphql\n  authorize: https://app.playerdata.co.uk/oauth/authorize\n  token: https://app.playerdata.co.uk/oauth/token\n  sign_out: https://app.playerdata.co.uk/api/auth/identities/sign_out\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playerdata/refs/heads/main/authentication/playerdata-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- Company
- Sports
- Sports Performance
- GPS Tracking
- Wearables
- Athlete Monitoring
- GraphQL
- Analytics
---
