---
api_key_in:
- header
api_specs:
- filename: langdock-openapi-original.yml
  format: yaml
  label: Langdock API
  slug: langdock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-openapi-original.yml
auth_types:
- http
description: Langdock authenticates every public API call with a workspace API key presented as an HTTP bearer token. There is no OAuth 2.0 or OpenID Connect surface on the public API — no /.well-known/openid-configuration or /.well-known/oauth-authorization-server is served (both 404). Keys are workspace-scoped, carry named product scopes, and are additionally bound to the specific agents and knowledge folders shared with them.
kind: authentication
layout: security
method: searched
name: Langdock Authentication
name_suffix: Authentication
oauth_flows: []
overview: Langdock secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Langdock
provider_slug: langdock
scheme_count: 1
schemes:
- applied: global — declared as the root-level security requirement for all operations
  bearerFormat: API Key
  description: API key as Bearer token. Format "Bearer [example key]"
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/langdock-openapi-original.yml
  type: http
slug: langdock-authentication
source_filename: langdock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/langdock-openapi-original.yml\ndocs: https://docs.langdock.com/en/developer/overview/api-introduction\ndescription: >-\n  Langdock authenticates every public API call with a workspace API key presented as\n  an HTTP bearer token. There is no OAuth 2.0 or OpenID Connect surface on the public\n  API — no /.well-known/openid-configuration or /.well-known/oauth-authorization-server\n  is served (both 404). Keys are workspace-scoped, carry named product scopes, and are\n  additionally bound to the specific agents and knowledge folders shared with them.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: API key as Bearer token. Format \"Bearer [example key]\"\n  sources:\n  - openapi/langdock-openapi-original.yml\n  applied: global — declared as the root-level security\
  \ requirement for all operations\nalternate_headers:\n- header: x-api-key\n  value: <api-key>\n  applies_to: Langdock Agent MCP Server (https://api.langdock.com/mcp)\n  source: https://docs.langdock.com/en/using-langdock/guides/integrations/mcp/langdock-agent-mcp-server\nkey_format:\n  prefix: sk-ld-\n  source: https://docs.langdock.com/en/admin/ai-adoption-and-rollout/best-practices/api-key-best-practices\nkey_management:\n  console: https://app.langdock.com/settings/workspace/products/api\n  path: Workspace Settings → Products → API\n  operations:\n  - create\n  - view\n  - revoke\n  environment_variable: LANGDOCK_API_KEY\n  rotation_guidance: >-\n    Langdock recommends rotating keys at least every 90 days, or immediately if\n    compromise is suspected.\n  docs: https://docs.langdock.com/en/admin/ai-adoption-and-rollout/best-practices/api-key-best-practices\nscopes:\n  model: >-\n    Langdock API keys carry named product scopes. Langdock does not publish a\n    consolidated scope reference\
  \ page; the scope names below are the ones evidenced\n    verbatim in the OpenAPI operation and error descriptions.\n  known:\n  - name: AGENT_API\n    evidence: 403 \"Insufficient permissions - requires AGENT_API scope\" on POST /assistant/v1/create\n    console_label: Agent API\n  - name: AUDIT_LOG_API\n    evidence: GET /audit-logs/{workspace_id} — \"Requires an API key with the `AUDIT_LOG_API`\n      scope.\"\n  unnamed:\n  - area: Skills\n    evidence: >-\n      Skills operations return 403 \"Missing required scope or access / create\n      permission / editor access / owner access\" but the scope name is not published.\nresource_sharing:\n  description: >-\n    Beyond scopes, access is granted per-resource: an agent or a knowledge folder must\n    be explicitly shared with an API key before that key can use it.\n  docs:\n  - https://docs.langdock.com/en/developer/agents-api/agent-api-guide\n  - https://docs.langdock.com/en/developer/knowledge-folder-api/sharing\nbrowser_restriction:\
  \ >-\n  API calls from browsers are blocked for security reasons; the API is backend-access\n  only.\noauth:\n  public_api: false\n  note: >-\n    OAuth appears inside the product as an authentication option for CUSTOM\n    INTEGRATIONS an admin configures — that is Langdock acting as an OAuth client\n    against third-party APIs, not an OAuth surface on the Langdock API itself. No\n    scopes/ artifact is emitted for this reason.\n  integrations_auth_docs: https://docs.langdock.com/en/developer/integrations-api/update-auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/authentication/langdock-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Enterprise AI
- LLM
- Agents
- Model Context Protocol
- Workflows
- Knowledge Management
- Germany
- Europe
---
