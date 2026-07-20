---
api_key_in: []
auth_types:
- oauth2
- session-token
description: ''
kind: authentication
layout: security
method: searched
name: Bullhorn Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Bullhorn secures its APIs with oauth2 and session-token across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Bullhorn
provider_slug: bullhorn
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://auth.bullhornstaffing.com/oauth/authorize
    flow: authorizationCode
    note: Host is data-center-specific; resolve via loginInfo oauthUrl. auth.bullhornstaffing.com is the default cluster.
    refresh: true
    tokenUrl: https://auth.bullhornstaffing.com/oauth/token
  name: OAuth2
  sources:
  - https://bullhorn.github.io/rest-api-docs/
  - live loginInfo
  type: oauth2
- expiry: session expires; refresh on 401; missing token yields 412 Precondition Failed
  in:
  - header
  - query
  - cookie
  name: BhRestToken
  obtained_via: GET https://rest.bullhornstaffing.com/login?access_token={oauth_access_token}&version=*
  parameter_name: BhRestToken
  scheme: session-token
  sources:
  - https://bullhorn.github.io/rest-api-docs/
  type: apiKey
  validation: GET {corpToken}/ping returns sessionExpires timestamp
slug: bullhorn-authentication
source_filename: bullhorn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://bullhorn.github.io/rest-api-docs/ + live loginInfo discovery\ndocs: https://bullhorn.github.io/rest-api-docs/\nsummary:\n  types: [oauth2, session-token]\n  oauth2_flows: [authorizationCode, refreshToken]\n  session_token: BhRestToken\n  notes: >-\n    Two-stage authentication. Stage 1 is standard OAuth 2.0 (authorization_code\n    grant with refresh_token) against the data-center OAuth endpoint. Stage 2\n    exchanges the OAuth access_token via the REST /login call for a short-lived\n    BhRestToken session token that authenticates all subsequent REST calls.\n    Bullhorn OAuth is session/user scoped and does NOT expose granular OAuth\n    scopes, so there is no scopes/ artifact.\ndiscovery:\n  endpoint: https://rest.bullhornstaffing.com/rest-services/loginInfo?username={API_Username}\n  returns: [oauthUrl, restUrl, atsUrl, coreUrl, novoUrl]\n  note: Clients must call loginInfo first to resolve the correct data-center\
  \ (swimlane) oauthUrl and restUrl; a 307 redirect is issued if the wrong data center is used.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.bullhornstaffing.com/oauth/authorize\n        tokenUrl: https://auth.bullhornstaffing.com/oauth/token\n        refresh: true\n        note: Host is data-center-specific; resolve via loginInfo oauthUrl. auth.bullhornstaffing.com is the default cluster.\n    sources: [https://bullhorn.github.io/rest-api-docs/, live loginInfo]\n  - name: BhRestToken\n    type: apiKey\n    scheme: session-token\n    in: [header, query, cookie]\n    parameter_name: BhRestToken\n    obtained_via: GET https://rest.bullhornstaffing.com/login?access_token={oauth_access_token}&version=*\n    validation: GET {corpToken}/ping returns sessionExpires timestamp\n    expiry: session expires; refresh on 401; missing token yields 412 Precondition Failed\n    sources: [https://bullhorn.github.io/rest-api-docs/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bullhorn/refs/heads/main/authentication/bullhorn-authentication.yml
summary_line: oauth2/session-token · 2 schemes
tags:
- Company
- Staffing
- Recruitment
- Applicant Tracking
- ATS
- CRM
- Human Resources
- REST
- OAuth
---
