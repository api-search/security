---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Skytap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skytap secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Skytap
provider_slug: skytap
scheme_count: 1
schemes:
- credential: username + API security token (or password)
  description: HTTP Basic authentication. Credentials are the account username plus an API security token (recommended) or the account password, base64-encoded as "<username>:<api-token>" in the Authorization header. The API security token is generated/rotated from the user account settings in the Skytap web UI.
  header: 'Authorization: Basic <base64(username:api-token)>'
  name: BasicAuth
  scheme: basic
  sources:
  - docs
  type: http
slug: skytap-authentication
source_filename: skytap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://help.skytap.com/api-quick-start.html\ndocs: https://help.skytap.com/api-quick-start.html\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication. Credentials are the account username plus an API\n      security token (recommended) or the account password, base64-encoded as\n      \"<username>:<api-token>\" in the Authorization header. The API security token\n      is generated/rotated from the user account settings in the Skytap web UI.\n    credential: username + API security token (or password)\n    header: 'Authorization: Basic <base64(username:api-token)>'\n    sources: [docs]\nnotes: >-\n  No OAuth2/OIDC or scope surface — authorization is account/role driven, not\n  scope-based, so scopes/ is intentionally omitted. Insufficient privileges most\n  often return\
  \ 404 (rather than 403) to avoid disclosing resource existence.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skytap/refs/heads/main/authentication/skytap-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cloud
- IBM Power
- Infrastructure as a Service
- Application Modernization
- Azure
- Virtual Machines
- DevOps
- REST API
---
