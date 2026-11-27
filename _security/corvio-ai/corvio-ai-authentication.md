---
anonymous_access: false
api_key_in: []
api_specs:
- filename: corvio-ai-agent-collaboration-api-openapi.yml
  format: yaml
  label: Corvio Agent collaboration API
  slug: corvio-ai-agent-collaboration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corvio-ai/openapi/corvio-ai-agent-collaboration-api-openapi.yml
- filename: corvio-ai-public-api-v1-api-openapi.yml
  format: yaml
  label: Corvio Public API v1 API
  slug: corvio-ai-public-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corvio-ai/openapi/corvio-ai-public-api-v1-api-openapi.yml
- filename: corvio-ai-public-api-v1-files-api-openapi.yml
  format: yaml
  label: Corvio Public API v1 - Files API
  slug: corvio-ai-public-api-v1-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corvio-ai/openapi/corvio-ai-public-api-v1-files-api-openapi.yml
- filename: corvio-ai-public-api-v1-local-markdown-sync-api-openapi.yml
  format: yaml
  label: Corvio Public API v1 - Local Markdown Sync API
  slug: corvio-ai-public-api-v1-local-markdown-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corvio-ai/openapi/corvio-ai-public-api-v1-local-markdown-sync-api-openapi.yml
- filename: corvio-ai-public-api-v1-source-publication-api-openapi.yml
  format: yaml
  label: Corvio Public API v1 - Source publication API
  slug: corvio-ai-public-api-v1-source-publication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corvio-ai/openapi/corvio-ai-public-api-v1-source-publication-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Corvio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Corvio secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Corvio
provider_slug: corvio-ai
scheme_count: 4
schemes:
- header: 'Authorization: Bearer $CORVIO_API_KEY'
  key_prefixes:
  - prefix: cvu_
    use: Workspace user API key (CORVIO_API_KEY)
  - prefix: cva_
    use: Short-lived read-only administrator key (CORVIO_ADMIN_API_KEY); "The stored key expires within seven days and remains separately revocable."
  - prefix: cvk_
    use: Legacy Workspace key; the docs say a 409 can mean a "legacy `cvk_` Workspace mismatch".
  name: CorvioApiKey
  note: '"Every call re-evaluates the key owner, Workspace membership, role, scope, ACL, expiry, and revocation."'
  scheme: bearer
  sources:
  - openapi/corvio-ai-openapi.yml
  - https://corvio.ai/developers/api
  type: http
- name: CorvioUploadCapability
  note: Declared in the OpenAPI securitySchemes for file-upload content transfer; the docs do not describe it separately.
  scheme: bearer
  sources:
  - openapi/corvio-ai-openapi.yml
  type: http
- name: Remote MCP OAuth
  note: Documented for the Remote MCP server at https://api.corvio.ai/mcp, not declared in the REST OpenAPI. llms.txt says OAuth "signs the user into an existing Corvio account and shows the named Agent identity that will act through this client".
  sources:
  - https://corvio.ai/llms.txt
  type: oauth2
- name: CLI device authorization
  note: '`corvio auth login` / `corvio-admin auth login` approve a single-use browser link (contract operations under /v1/auth/device-authorizations and /v1/auth/device-token). These were read from docs only; not called.'
  sources:
  - https://corvio.ai/developers/cli
  type: device-link
slug: corvio-ai-authentication
source_filename: corvio-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://corvio.ai/developers/api\ndocs: https://corvio.ai/developers/api\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: CorvioApiKey\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer $CORVIO_API_KEY'\n  key_prefixes:\n  - prefix: cvu_\n    use: Workspace user API key (CORVIO_API_KEY)\n  - prefix: cva_\n    use: Short-lived read-only administrator key (CORVIO_ADMIN_API_KEY); \"The stored\n      key expires within seven days and remains separately revocable.\"\n  - prefix: cvk_\n    use: Legacy Workspace key; the docs say a 409 can mean a \"legacy `cvk_` Workspace\n      mismatch\".\n  note: '\"Every call re-evaluates the key owner, Workspace membership, role, scope,\n    ACL, expiry, and revocation.\"'\n  sources:\n  - openapi/corvio-ai-openapi.yml\n  - https://corvio.ai/developers/api\n- name: CorvioUploadCapability\n  type: http\n  scheme: bearer\n  note: Declared in the OpenAPI securitySchemes\
  \ for file-upload content transfer;\n    the docs do not describe it separately.\n  sources:\n  - openapi/corvio-ai-openapi.yml\n- name: Remote MCP OAuth\n  type: oauth2\n  note: Documented for the Remote MCP server at https://api.corvio.ai/mcp, not declared\n    in the REST OpenAPI. llms.txt says OAuth \"signs the user into an existing Corvio\n    account and shows the named Agent identity that will act through this client\".\n  sources:\n  - https://corvio.ai/llms.txt\n- name: CLI device authorization\n  type: device-link\n  note: '`corvio auth login` / `corvio-admin auth login` approve a single-use browser\n    link (contract operations under /v1/auth/device-authorizations and /v1/auth/device-token).\n    These were read from docs only; not called.'\n  sources:\n  - https://corvio.ai/developers/cli\ndocs_pages:\n- https://corvio.ai/developers/cli\n- https://corvio.ai/developers/admin-cli\n- https://corvio.ai/developers/skills/corvio-operate-workspace/references/api.md\n"
source_yaml_url: https://artifacts.apis.io/corvio-ai/authentication/corvio-ai-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Company
- Artificial Intelligence
- Notes
- Knowledge Management
- Workspace
- AI Agents
- MCP
- Developer API
- CLI
---
