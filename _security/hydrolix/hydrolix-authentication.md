---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hydrolix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hydrolix secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hydrolix
provider_slug: hydrolix
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Bearer token obtained by logging in with Hydrolix credentials against the Config API.
  name: bearerAuth
  scheme: bearer
  sources:
  - docs.hydrolix.io Config API reference
  type: http
- description: Long-lived service-account token for automated / scripted access (hdxcli, MCP server).
  name: serviceAccount
  scheme: bearer
  sources:
  - github.com/hydrolix/hdxcli
  type: http
slug: hydrolix-authentication
source_filename: hydrolix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.hydrolix.io/latest/openapi/ + https://github.com/hydrolix/hdxcli\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  credential_login: true\n  service_accounts: true\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  Hydrolix is deployed per-customer (BYOC on AWS/GCP/Kubernetes), so there is no single public\n  API host — the base host is your own cluster hostname. The Config API authenticates with\n  Hydrolix user credentials (username/password) exchanged for a bearer token, presented as an\n  Authorization: Bearer header on subsequent requests. Service Accounts provide long-lived,\n  non-interactive tokens for automation (used by hdxcli and the MCP server). No public OAuth2\n  authorization-server or API-key scheme is documented.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token obtained by logging in with Hydrolix credentials against\
  \ the Config API.\n    sources: [docs.hydrolix.io Config API reference]\n  - name: serviceAccount\n    type: http\n    scheme: bearer\n    description: Long-lived service-account token for automated / scripted access (hdxcli, MCP server).\n    sources: [github.com/hydrolix/hdxcli]\ndocs: https://docs.hydrolix.io/latest/openapi/config-api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydrolix/refs/heads/main/authentication/hydrolix-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Observability
- Log Analytics
- Data Lake
- Streaming
- ClickHouse
- Monitoring
- Time Series
---
