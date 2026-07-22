---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Starburst Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Starburst secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Starburst
provider_slug: starburst
scheme_count: 3
schemes:
- description: 'Starburst Galaxy public API uses the OAuth2 client credentials flow. A base64-encoded clientId:clientSecret is exchanged at /oauth/v2/token for a bearer access token that expires after 10 minutes. The token is sent as `Authorization: Bearer <token>`.'
  flow: clientCredentials
  name: galaxyOAuth2
  scheme: oauth2
  sources:
  - docs.starburst.io/starburst-galaxy/developer-tools/api
  token_ttl_seconds: 600
  token_url: https://<account>.galaxy.starburst.io/oauth/v2/token
  type: oauth2
- description: Bearer access token obtained from the Galaxy OAuth2 token endpoint.
  name: galaxyBearer
  scheme: bearer
  sources:
  - docs.starburst.io/starburst-galaxy/developer-tools/api
  type: http
- description: Starburst Enterprise REST API accepts HTTP Basic auth (base64 credentials) or bearer token auth using the same token as the web UI; the active role is selected via the X-Trino-Role header.
  name: enterpriseBasic
  scheme: basic
  sources:
  - docs.starburst.io/latest/starburst-rest-api.html
  type: http
slug: starburst-authentication
source_filename: starburst-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.starburst.io/starburst-galaxy/developer-tools/api/index.html\ndocs: https://docs.starburst.io/starburst-galaxy/developer-tools/api/index.html\nsummary:\n  types: [oauth2, http]\n  oauth2_flows: [clientCredentials]\n  http_schemes: [bearer, basic]\nschemes:\n  - name: galaxyOAuth2\n    type: oauth2\n    scheme: oauth2\n    flow: clientCredentials\n    token_url: https://<account>.galaxy.starburst.io/oauth/v2/token\n    token_ttl_seconds: 600\n    description: >-\n      Starburst Galaxy public API uses the OAuth2 client credentials flow. A base64-encoded\n      clientId:clientSecret is exchanged at /oauth/v2/token for a bearer access token that\n      expires after 10 minutes. The token is sent as `Authorization: Bearer <token>`.\n    sources: [docs.starburst.io/starburst-galaxy/developer-tools/api]\n  - name: galaxyBearer\n    type: http\n    scheme: bearer\n    description: Bearer access token obtained from the\
  \ Galaxy OAuth2 token endpoint.\n    sources: [docs.starburst.io/starburst-galaxy/developer-tools/api]\n  - name: enterpriseBasic\n    type: http\n    scheme: basic\n    description: >-\n      Starburst Enterprise REST API accepts HTTP Basic auth (base64 credentials) or bearer\n      token auth using the same token as the web UI; the active role is selected via the\n      X-Trino-Role header.\n    sources: [docs.starburst.io/latest/starburst-rest-api.html]\nnotes: >-\n  Galaxy uses OAuth2 client-credentials (no granular OAuth scopes documented; access is governed\n  by role/privilege services), so no scopes/ artifact is emitted. Enterprise uses Basic/Bearer +\n  X-Trino-Role role selection backed by built-in access control.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starburst/refs/heads/main/authentication/starburst-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Company
- Data Analytics
- Data Lakehouse
- SQL Query Engine
- Trino
- Federated Query
- Data Governance
- Business Intelligence
---
