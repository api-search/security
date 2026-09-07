---
anonymous_access: false
api_key_in: []
api_specs:
- filename: workera-api-openapi.json
  format: json
  label: Workera API
  slug: workera-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workera/refs/heads/main/openapi/workera-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Workera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Workera secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Workera
provider_slug: workera
scheme_count: 1
schemes:
- applied: global
  example: 'curl -H "Content-Type: application/json" -H "authorization: Bearer YOUR_KEY" https://skills.workera.ai/api/v1/ping'
  header: authorization
  location: header
  name: authorization
  scheme: bearer
  sources:
  - openapi/workera-api-openapi.json
  - https://skills.workera.ai/api/docs
  type: http
  value_format: Bearer YOUR_KEY
slug: workera-authentication
source_filename: workera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://skills.workera.ai/api/docs\nderived_from: openapi/workera-api-openapi.json\nsummary:\n  types:\n  - http\n  primary: bearer API key\n  oauth2: false\n  note: >-\n    Two distinct auth models exist at Workera. The REST API uses a static, company-scoped bearer API\n    key. The remote MCP server at https://skills.workera.ai/mcp uses OAuth 2.0 with dynamic client\n    registration (see mcp/workera-mcp.yml and well-known/workera-oauth-authorization-server.json).\nschemes:\n- name: authorization\n  type: http\n  scheme: bearer\n  applied: global\n  location: header\n  header: authorization\n  value_format: 'Bearer YOUR_KEY'\n  example: >-\n    curl -H \"Content-Type: application/json\" -H \"authorization: Bearer YOUR_KEY\"\n    https://skills.workera.ai/api/v1/ping\n  sources:\n  - openapi/workera-api-openapi.json\n  - https://skills.workera.ai/api/docs\nkey_issuance:\n  self_serve: false\n  process: >-\n    API keys are\
  \ tied to a Workera company/organization, are available only to enterprise customers,\n    and are issued on request through the customer's Workera CSM. There is no public developer signup\n    that yields an API key.\n  rotation: not_documented\nscopes:\n  model: key-restricted scopes\n  enforcement: >-\n    API keys can be restricted by scope. Endpoints that require a scope return HTTP 403 when the scope\n    is missing.\n  known_scopes:\n  - name: audit_events\n    required_by:\n    - GET /api/v1/audit_events\n    evidence: https://skills.workera.ai/api/docs\n  note: >-\n    Workera documents that scopes exist and names one (audit_events) but publishes no full scope\n    reference. This is NOT an OAuth 2.0 scope surface, so scopes/workera-scopes.yml is intentionally\n    absent; the scope model belongs to the API key.\ntransport:\n  https_required: true\n  statement: All API requests must be made authenticated and sent over HTTPS.\nmcp_authorization:\n  endpoint: https://skills.workera.ai/mcp\n\
  \  model: oauth2\n  issuer: https://skills.workera.ai\n  authorization_endpoint: https://skills.workera.ai/mcp/oauth/authorize\n  token_endpoint: https://skills.workera.ai/mcp/oauth/token\n  registration_endpoint: https://skills.workera.ai/mcp/oauth/register\n  grant_types:\n  - authorization_code\n  - refresh_token\n  pkce:\n  - S256\n  scopes_supported:\n  - mcp\n  discovery:\n  - https://skills.workera.ai/.well-known/oauth-authorization-server\n  - https://skills.workera.ai/.well-known/oauth-protected-resource/mcp\nwebhook_authentication:\n  mechanism: HMAC-SHA256 request signature\n  header: X-Workera-Signature\n  format: 'sha256=<hex digest of the raw request body keyed with the shared webhook secret>'\n  secret_provisioning: configured per company through the Workera CSM\n  source: https://skills.workera.ai/api/docs\nevidence:\n- url: https://skills.workera.ai/api/docs\n  status: 200\n- url: https://skills.workera.ai/api/docs/openapi\n  status: 200\n- url: https://skills.workera.ai/api/v1\n\
  \  status: 401\n  body: '{\"code\":\"unauthorized\",\"message\":\"You are not authorized to access this resource. Please provide a valid API key.\",\"type\":\"invalid_request_error\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workera/refs/heads/main/authentication/workera-authentication.yml
summary_line: http · 1 scheme
tags:
- Skills Intelligence
- Skills Assessment
- Human Resources
- Learning and Development
- Talent Management
- Workforce Analytics
- Artificial Intelligence
- Benchmarking
- Enterprise Software
- MCP
- Company
---
