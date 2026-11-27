---
anonymous_access: false
api_key_in: []
api_specs:
- filename: createya-ai-balance-api-openapi.yml
  format: yaml
  label: Createya Balance API
  slug: createya-ai-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-balance-api-openapi.yml
- filename: createya-ai-healthz-api-openapi.yml
  format: yaml
  label: Createya Healthz API
  slug: createya-ai-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-healthz-api-openapi.yml
- filename: createya-ai-mcp-api-openapi.yml
  format: yaml
  label: Createya MCP API
  slug: createya-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-mcp-api-openapi.yml
- filename: createya-ai-models-api-openapi.yml
  format: yaml
  label: Createya Models API
  slug: createya-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-models-api-openapi.yml
- filename: createya-ai-run-api-openapi.yml
  format: yaml
  label: Createya Run API
  slug: createya-ai-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-run-api-openapi.yml
- filename: createya-ai-runs-api-openapi.yml
  format: yaml
  label: Createya Runs API
  slug: createya-ai-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-runs-api-openapi.yml
- filename: createya-ai-uploads-api-openapi.yml
  format: yaml
  label: Createya Uploads API
  slug: createya-ai-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-uploads-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Createya Authentication
name_suffix: Authentication
oauth_flows: []
overview: Createya secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Createya
provider_slug: createya-ai
scheme_count: 2
schemes:
- description: 'API key: crya_sk_<hex>'
  header: 'Authorization: Bearer crya_sk_live_...'
  isolation: A key is bound to one workspace and cannot spend credits from another.
  issuance: Created at createya.ai/settings/api-keys ("Create new key"); shown once.
  key_format: crya_sk_live_<32 hex>
  name: BearerAuth
  prefixes:
  - prefix: crya_sk_live_
    purpose: Production key; credits are charged to the workspace the key is bound to.
  - prefix: crya_sk_test_
    purpose: Test keys - documented as not yet issued publicly.
  restrictions: Keys may carry allowed_ips and allowed_models whitelists and scopes (generate / read:usage), per the error reference (https://github.com/Createya-ai/createya-mcp/blob/main/examples/10-error-handling.md).
  rotation: Revoke the old key at createya.ai/settings/api-keys (takes effect immediately), then create a new key.
  scheme: bearer
  sources:
  - openapi/createya-ai-openapi.yml
  - https://docs.createya.ai/authentication
  storage: Docs state keys are stored server-side with bcrypt and the raw value is not retrievable.
  type: http
- applies_to: https://api.createya.ai/mcp
  description: OAuth 2.1 + PKCE for Claude.ai / Claude Desktop connecting to the MCP endpoint https://api.createya.ai/mcp; the key is entered once on the Createya authorization page. Other MCP clients (Cursor, Cline, Windsurf, Codex, OpenCode) use the Bearer header.
  name: MCP OAuth
  sources:
  - https://docs.createya.ai/authentication
  - https://github.com/Createya-ai/createya-mcp/blob/main/CHANGELOG.md
  type: oauth2
slug: createya-ai-authentication
source_filename: createya-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.createya.ai/authentication\ndocs: https://docs.createya.ai/authentication\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key: crya_sk_<hex>'\n  key_format: crya_sk_live_<32 hex>\n  prefixes:\n  - prefix: crya_sk_live_\n    purpose: Production key; credits are charged to the workspace the key is bound to.\n  - prefix: crya_sk_test_\n    purpose: Test keys - documented as not yet issued publicly.\n  header: 'Authorization: Bearer crya_sk_live_...'\n  issuance: Created at createya.ai/settings/api-keys (\"Create new key\"); shown once.\n  storage: Docs state keys are stored server-side with bcrypt and the raw value is not retrievable.\n  rotation: Revoke the old key at createya.ai/settings/api-keys (takes effect immediately), then create a new key.\n  isolation: A key is bound to one workspace and cannot spend credits from another.\n  restrictions:\
  \ Keys may carry allowed_ips and allowed_models whitelists and scopes (generate / read:usage), per the error reference (https://github.com/Createya-ai/createya-mcp/blob/main/examples/10-error-handling.md).\n  sources:\n  - openapi/createya-ai-openapi.yml\n  - https://docs.createya.ai/authentication\n- name: MCP OAuth\n  type: oauth2\n  description: OAuth 2.1 + PKCE for Claude.ai / Claude Desktop connecting to the MCP endpoint https://api.createya.ai/mcp; the key is entered once on the Createya authorization page. Other MCP clients (Cursor, Cline, Windsurf, Codex, OpenCode) use the Bearer header.\n  applies_to: https://api.createya.ai/mcp\n  sources:\n  - https://docs.createya.ai/authentication\n  - https://github.com/Createya-ai/createya-mcp/blob/main/CHANGELOG.md\n"
source_yaml_url: https://artifacts.apis.io/createya-ai/authentication/createya-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Generative AI
- Image Generation
- Video Generation
- Audio Generation
- Model Aggregator
- MCP
---
