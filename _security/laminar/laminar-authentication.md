---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Laminar Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
overview: Laminar secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode flow(s).
provider_name: Laminar
provider_slug: laminar
scheme_count: 2
schemes:
- env_var: LMNR_PROJECT_API_KEY
  format: Bearer <project_api_key>
  header: Authorization
  in: header
  issued_at: Laminar dashboard -> Settings -> Project API Keys
  minted_by_cli: lmnr-cli setup mints a project API key and writes LMNR_PROJECT_API_KEY to .env.local or .env
  name: ProjectApiKeyBearer
  revocation: keys stay visible and revocable in Settings -> Project API Keys
  scheme: bearer
  scope: project-scoped; every request is automatically constrained to the owning project so no tenant filter is required in queries
  type: http
  used_by:
  - POST /v1/sql/query (SQL Query API)
  - /v1/traces (OTLP trace ingest)
  - /v1/mcp (MCP server)
  - '@lmnr-ai/lmnr and lmnr Python SDKs (Laminar.initialize / LaminarClient)'
- credential_store: ~/.config/lmnr/credentials.json (precedence $XDG_CONFIG_HOME, %APPDATA%, ~/.config)
  description: 'lmnr-cli authenticates as the signed-in user, not with a project API key. lmnr-cli login starts an OAuth device flow: the CLI prints a verification URL and code and opens the browser for approval.'
  flow: deviceCode
  name: CliDeviceFlow
  revocation: revoked sessions require re-running lmnr-cli login; lmnr-cli logout removes stored credentials
  self_hosted: login targets the frontend (auth issuer) via LMNR_FRONTEND_URL or --frontend-url
  token_lifetime: short-lived access token, refreshed automatically as it nears expiry
  type: oauth2
slug: laminar-authentication
source_filename: laminar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://laminar.sh/docs/platform/cli + https://laminar.sh/docs/platform/mcp +\n  https://github.com/lmnr-ai/lmnr-skills/blob/main/skills/laminar/references/sql-query-api.md\ndocs: https://laminar.sh/docs/platform/cli#authenticate\nnote: Laminar publishes no OpenAPI, so this profile is searched from the documentation rather than\n  derived from securitySchemes.\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - deviceCode\n  credential_kinds:\n  - project API key (machine/SDK/MCP/HTTP API)\n  - user session via OAuth device flow (CLI)\nschemes:\n- name: ProjectApiKeyBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <project_api_key>'\n  env_var: LMNR_PROJECT_API_KEY\n  issued_at: Laminar dashboard -> Settings -> Project API Keys\n  minted_by_cli: 'lmnr-cli setup mints a project API key and writes LMNR_PROJECT_API_KEY to .env.local\n    or\
  \ .env'\n  scope: project-scoped; every request is automatically constrained to the owning project so no tenant\n    filter is required in queries\n  used_by:\n  - POST /v1/sql/query (SQL Query API)\n  - /v1/traces (OTLP trace ingest)\n  - /v1/mcp (MCP server)\n  - '@lmnr-ai/lmnr and lmnr Python SDKs (Laminar.initialize / LaminarClient)'\n  revocation: keys stay visible and revocable in Settings -> Project API Keys\n- name: CliDeviceFlow\n  type: oauth2\n  flow: deviceCode\n  description: 'lmnr-cli authenticates as the signed-in user, not with a project API key. lmnr-cli\n    login starts an OAuth device flow: the CLI prints a verification URL and code and opens the\n    browser for approval.'\n  credential_store: ~/.config/lmnr/credentials.json (precedence $XDG_CONFIG_HOME, %APPDATA%,\n    ~/.config)\n  token_lifetime: short-lived access token, refreshed automatically as it nears expiry\n  revocation: revoked sessions require re-running lmnr-cli login; lmnr-cli logout removes stored\n\
  \    credentials\n  self_hosted: login targets the frontend (auth issuer) via LMNR_FRONTEND_URL or --frontend-url\nproject_resolution:\n  description: CLI data commands resolve which project they target from the working directory rather\n    than from the credential.\n  order:\n  - --project-id <id> flag\n  - nearest .lmnr/project.json walking up from the current directory\n  link_file: .lmnr/project.json (holds project id and display details, never secrets)\nself_hosting:\n  base_url_env: LMNR_BASE_URL\n  frontend_url_env: LMNR_FRONTEND_URL\n  default_http_port: 8000\n  default_grpc_port: 8001\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laminar/refs/heads/main/authentication/laminar-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Observability
- LLM
- AI Agents
- Tracing
- OpenTelemetry
- Evaluations
- Monitoring
- Developer Tools
- Open Source
---
