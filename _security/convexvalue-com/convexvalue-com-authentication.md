---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ConvexValue Authentication
name_suffix: Authentication
oauth_flows: []
overview: ConvexValue secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ConvexValue
provider_slug: convexvalue-com
scheme_count: 1
schemes:
- applies_to:
  - https://tap.convexvalue.com/api/data
  - https://tap.convexvalue.com/api/data/mcp
  description: Every request needs a data API key (cv_live_…) as a Bearer token. Personal API keys are a Go and Research plan feature, created and revoked on the account page; the full key is shown once at creation. Keys can be named and revoked independently; usage and rate limits are counted per user, so multiple keys share one quota. Inside the desktop app a key is provisioned automatically and injected server-side via a local proxy.
  docs:
  - https://cvforge.convexvalue.com/docs/api
  - https://cvforge.convexvalue.com/docs/api/mcp
  header: Authorization
  in: header
  key_prefix: cv_live_
  name: bearerApiKey
  scheme: bearer
  type: http
slug: convexvalue-com-authentication
source_filename: convexvalue-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cvforge.convexvalue.com/docs/api\ndocs: https://cvforge.convexvalue.com/docs/api\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: Every request needs a data API key (cv_live_…) as a Bearer token. Personal API keys are a Go and\n    Research plan feature, created and revoked on the account page; the full key is shown once at creation. Keys\n    can be named and revoked independently; usage and rate limits are counted per user, so multiple keys share one\n    quota. Inside the desktop app a key is provisioned automatically and injected server-side via a local proxy.\n  key_prefix: cv_live_\n  applies_to:\n  - https://tap.convexvalue.com/api/data\n  - https://tap.convexvalue.com/api/data/mcp\n  docs:\n  - https://cvforge.convexvalue.com/docs/api\n  - https://cvforge.convexvalue.com/docs/api/mcp\nnotes: 'MCP server: a bad\
  \ key is a 401 before the body is parsed; past auth, errors ride inside the JSON-RPC body.\n  No OAuth is documented.'\n"
source_yaml_url: https://artifacts.apis.io/convexvalue-com/authentication/convexvalue-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Financial Data
- Options Analytics
- Market Data
- Stocks
- Trading
- MCP
- Artificial Intelligence
---
