---
anonymous_access: false
api_key_in:
- header
- cookie
api_specs:
- filename: n8n-public-api-openapi.yml
  format: yaml
  label: N8n
  slug: n8n
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-public-api-openapi.yml
- filename: n8n-audit-api-openapi.yml
  format: yaml
  label: N8n Audit API
  slug: n8n-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-audit-api-openapi.yml
- filename: n8n-communitypackage-api-openapi.yml
  format: yaml
  label: N8n CommunityPackage API
  slug: n8n-communitypackage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-communitypackage-api-openapi.yml
- filename: n8n-credential-api-openapi.yml
  format: yaml
  label: N8n Credential API
  slug: n8n-credential-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-credential-api-openapi.yml
- filename: n8n-datatable-api-openapi.yml
  format: yaml
  label: N8n DataTable API
  slug: n8n-datatable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-datatable-api-openapi.yml
- filename: n8n-discover-api-openapi.yml
  format: yaml
  label: N8n Discover API
  slug: n8n-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-discover-api-openapi.yml
- filename: n8n-execution-api-openapi.yml
  format: yaml
  label: N8n Execution API
  slug: n8n-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-execution-api-openapi.yml
- filename: n8n-folders-api-openapi.yml
  format: yaml
  label: N8n Folders API
  slug: n8n-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-folders-api-openapi.yml
- filename: n8n-insights-api-openapi.yml
  format: yaml
  label: N8n Insights API
  slug: n8n-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-insights-api-openapi.yml
- filename: n8n-projects-api-openapi.yml
  format: yaml
  label: N8n Projects API
  slug: n8n-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-projects-api-openapi.yml
- filename: n8n-sourcecontrol-api-openapi.yml
  format: yaml
  label: N8n SourceControl API
  slug: n8n-sourcecontrol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-sourcecontrol-api-openapi.yml
- filename: n8n-tags-api-openapi.yml
  format: yaml
  label: N8n Tags API
  slug: n8n-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-tags-api-openapi.yml
- filename: n8n-user-api-openapi.yml
  format: yaml
  label: N8n User API
  slug: n8n-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-user-api-openapi.yml
- filename: n8n-variables-api-openapi.yml
  format: yaml
  label: N8n Variables API
  slug: n8n-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-variables-api-openapi.yml
- filename: n8n-workflow-api-openapi.yml
  format: yaml
  label: N8n Workflow API
  slug: n8n-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-workflow-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: N8N Authentication
name_suffix: Authentication
oauth_flows: []
overview: n8n secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: n8n
provider_slug: n8n
scheme_count: 3
schemes:
- description: Primary public-API authentication; key created under Settings > n8n API.
  in: header
  name: ApiKeyAuth
  parameter: X-N8N-API-KEY
  sources:
  - openapi/n8n-public-api-openapi.yml
  - https://docs.n8n.io/connect/n8n-api/authentication
  type: apiKey
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/n8n-public-api-openapi.yml
  type: http
- description: Browser-session cookie auth (used by the instance UI).
  in: cookie
  name: CookieAuth
  parameter: n8n-auth
  sources:
  - openapi/n8n-public-api-openapi.yml
  type: apiKey
slug: n8n-authentication
source_filename: n8n-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\ndocs: https://docs.n8n.io/connect/n8n-api/authentication\nsource: >-\n  https://docs.n8n.io/connect/n8n-api/authentication.md +\n  openapi/n8n-public-api-openapi.yml (provider-published contract)\nsummary:\n  types:\n    - apiKey\n    - http\n  api_key_in:\n    - header\n    - cookie\nnotes: >-\n  API keys are created in Settings > n8n API with a label and expiration; on\n  Enterprise plans keys can be restricted to scopes (see scopes/n8n-scopes.yml).\n  The API is not available during the free Cloud trial. The instance-level MCP\n  server authenticates separately via OAuth (recommended) or a bearer personal\n  access token.\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: X-N8N-API-KEY\n    description: Primary public-API authentication; key created under Settings > n8n API.\n    sources:\n      - openapi/n8n-public-api-openapi.yml\n      - https://docs.n8n.io/connect/n8n-api/authentication\n  - name:\
  \ BearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    sources:\n      - openapi/n8n-public-api-openapi.yml\n  - name: CookieAuth\n    type: apiKey\n    in: cookie\n    parameter: n8n-auth\n    description: Browser-session cookie auth (used by the instance UI).\n    sources:\n      - openapi/n8n-public-api-openapi.yml\nmcp_auth:\n  methods: [oauth, bearer-token]\n  docs: https://docs.n8n.io/connect/connect-to-n8n-mcp-server/\n  note: OAuth with per-client permissions and scope selection at consent (n8n 2.32+); tokens rotatable, revocation per client.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/authentication/n8n-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Agents
- Artificial Intelligence
- Integration
- Workflows
- Automation
- Low Code
---
