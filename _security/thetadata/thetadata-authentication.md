---
api_key_in:
- cli-argument
- environment-variable
- dotenv-file
api_specs:
- filename: thetadata-streaming-asyncapi.yml
  format: yaml
  label: ThetaData Streaming WebSocket API
  slug: thetadata-streaming-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/asyncapi/thetadata-streaming-asyncapi.yml
- filename: thetadata-calendar-api-openapi.yml
  format: yaml
  label: ThetaData Calendar API
  slug: thetadata-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-calendar-api-openapi.yml
- filename: thetadata-index-api-openapi.yml
  format: yaml
  label: ThetaData Index API
  slug: thetadata-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-index-api-openapi.yml
- filename: thetadata-interest-rate-api-openapi.yml
  format: yaml
  label: ThetaData Interest Rate API
  slug: thetadata-interest-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-interest-rate-api-openapi.yml
- filename: thetadata-option-api-openapi.yml
  format: yaml
  label: ThetaData Option API
  slug: thetadata-option-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-option-api-openapi.yml
- filename: thetadata-stock-api-openapi.yml
  format: yaml
  label: ThetaData Stock API
  slug: thetadata-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/openapi/thetadata-stock-api-openapi.yml
auth_types:
- apiKey
- credentials
description: 'ThetaData authenticates at the session level, not per HTTP request. The published OpenAPI declares security: [] because the local REST API served by the Theta Terminal (127.0.0.1:25503/v3) is an unauthenticated loopback surface; credentials are supplied when the terminal (or the Python library client) starts, which opens an authenticated session to ThetaData''s MDDS servers. Requests are additionally IP-pinned to the first requester (error 476 WRONG_IP) and a single terminal session is enforced (error 478 INVALID_SESSION_ID).'
kind: authentication
layout: security
method: searched
name: Thetadata Authentication
name_suffix: Authentication
oauth_flows: []
overview: ThetaData secures its APIs with apiKey and credentials across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ThetaData
provider_slug: thetadata
scheme_count: 2
schemes:
- delivery:
  - example: java -jar ThetaTerminalv3.jar --api-key <key>
    method: cli-argument
  - method: environment-variable
    name: THETADATA_API_KEY
  - method: dotenv-file
    notes: .env next to ThetaTerminalv3.jar (or --dotenv-dir), containing THETADATA_API_KEY
  description: API key generated from the user portal (https://thetadata.net/portal). Requires Theta Terminal version 20260615+ or Python library 1.0.9+.
  name: api_key
  priority: CLI argument, then environment variable, then .env file
  provisioning: https://thetadata.net/portal
  type: apiKey
- description: Account email + password as an alternative to an API key. Terminal reads creds.txt (email line 1, password line 2) next to the JAR or via --creds-file; the Python library accepts email/password arguments, a creds_file path, or the THETADATA_CREDENTIALS_FILE environment variable.
  name: credentials
  type: credentials
slug: thetadata-authentication
source_filename: thetadata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: >-\n  https://docs.thetadata.us/Articles/Getting-Started/Getting-Started.html\n  (Authentication section) and\n  https://docs.thetadata.us/Python-Library/Getting-Started.html.\ndocs: https://docs.thetadata.us/Articles/Getting-Started/Getting-Started.html\ndescription: >-\n  ThetaData authenticates at the session level, not per HTTP request. The\n  published OpenAPI declares security: [] because the local REST API served by\n  the Theta Terminal (127.0.0.1:25503/v3) is an unauthenticated loopback\n  surface; credentials are supplied when the terminal (or the Python library\n  client) starts, which opens an authenticated session to ThetaData's MDDS\n  servers. Requests are additionally IP-pinned to the first requester (error\n  476 WRONG_IP) and a single terminal session is enforced (error 478\n  INVALID_SESSION_ID).\nsummary:\n  types: [apiKey, credentials]\n  applied_at: session (Theta Terminal launch / ThetaClient construction),\
  \ not per-request\n  api_key_in: [cli-argument, environment-variable, dotenv-file]\n  oauth2_flows: []\nschemes:\n  - name: api_key\n    type: apiKey\n    description: >-\n      API key generated from the user portal (https://thetadata.net/portal).\n      Requires Theta Terminal version 20260615+ or Python library 1.0.9+.\n    provisioning: https://thetadata.net/portal\n    delivery:\n      - method: cli-argument\n        example: java -jar ThetaTerminalv3.jar --api-key <key>\n      - method: environment-variable\n        name: THETADATA_API_KEY\n      - method: dotenv-file\n        notes: .env next to ThetaTerminalv3.jar (or --dotenv-dir), containing THETADATA_API_KEY\n    priority: CLI argument, then environment variable, then .env file\n  - name: credentials\n    type: credentials\n    description: >-\n      Account email + password as an alternative to an API key. Terminal reads\n      creds.txt (email line 1, password line 2) next to the JAR or via\n      --creds-file; the Python\
  \ library accepts email/password arguments, a\n      creds_file path, or the THETADATA_CREDENTIALS_FILE environment variable.\npython_library:\n  priority: >-\n    Explicit creds_file, then API key (api_key argument or THETADATA_API_KEY,\n    including .env), then email/password arguments, then default creds.txt.\n  transport: Authenticates over HTTPS; requests data over gRPC (no terminal needed).\nlocal_rest_api:\n  scheme: none (loopback)\n  notes: >-\n    openapi security is empty by design — only the local machine can reach the\n    terminal's HTTP server; entitlements are enforced server-side per\n    subscription (error 471 PERMISSION).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thetadata/refs/heads/main/authentication/thetadata-authentication.yml
summary_line: apiKey/credentials · 2 schemes
tags:
- Financial
- Market Data
- Options
- Stocks
- Indices
- Real-Time
- Historical Data
- Trading
---
