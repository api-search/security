---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Moveinsync Authentication
name_suffix: Authentication
oauth_flows: []
overview: MoveInSync secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MoveInSync
provider_slug: moveinsync
scheme_count: 2
schemes:
- endpoint: https://api.moveinsync.com/auth/token
  grant_type: client_credentials
  name: BasicAuth
  notes: Username and password are provisioned by MoveInSync for production access. Posted to the token endpoint with grant_type=client_credentials.
  scheme: basic
  sources:
  - https://helpcenter.moveinsync.com/support/solutions/articles/1070000134479-auth-api
  type: http
  used_for: token issuance
- bearerFormat: JWT
  name: BearerJWT
  notes: The JWT returned by the token endpoint is sent in the Authorization header as `Bearer <token>` on subsequent API requests. Expires every 24 hours.
  scheme: bearer
  sources:
  - https://helpcenter.moveinsync.com/support/solutions/articles/1070000134479-auth-api
  token_ttl_seconds: 86400
  type: http
  used_for: API and webhook calls
slug: moveinsync-authentication
source_filename: moveinsync-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://helpcenter.moveinsync.com/support/solutions/articles/1070000134479-auth-api\ndocs: https://helpcenter.moveinsync.com/support/solutions/articles/1070000134479-auth-api\nsummary:\n  types: [http, oauth2]\n  description: >-\n    MoveInSync exposes a two-legged machine-to-machine auth flow. Integration\n    partners exchange an issued username/password (HTTP Basic) with an OAuth2\n    client-credentials grant at the token endpoint to obtain a JWT access\n    token, then present that JWT as a Bearer token on all API and webhook\n    calls. Tokens expire every 24 hours and must be refreshed.\nschemes:\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    used_for: token issuance\n    endpoint: https://api.moveinsync.com/auth/token\n    grant_type: client_credentials\n    notes: >-\n      Username and password are provisioned by MoveInSync for production\n      access. Posted to the token endpoint with grant_type=client_credentials.\n\
  \    sources: [https://helpcenter.moveinsync.com/support/solutions/articles/1070000134479-auth-api]\n  - name: BearerJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    used_for: API and webhook calls\n    token_ttl_seconds: 86400\n    notes: >-\n      The JWT returned by the token endpoint is sent in the Authorization\n      header as `Bearer <token>` on subsequent API requests. Expires every\n      24 hours.\n    sources: [https://helpcenter.moveinsync.com/support/solutions/articles/1070000134479-auth-api]\nhost: https://api.moveinsync.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moveinsync/refs/heads/main/authentication/moveinsync-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Vertical Software
- Transportation
- Employee Commute
- Mobility
- Fleet Management
- Parking
- Workplace Management
- Ridesharing
- Logistics
---
