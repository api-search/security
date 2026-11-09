---
anonymous_access: false
api_key_in: []
api_specs:
- filename: contextlm-top-openapi-generated.yml
  format: yaml
  label: ContextLM API
  slug: contextlm-top-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contextlm-top/openapi/_ae-authored/contextlm-top-openapi-generated.yml
auth_types: []
description: Authentication schemes for ContextLM API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Contextlm Top Authentication
name_suffix: Authentication
oauth_flows: []
overview: ContextLM declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ContextLM
provider_slug: contextlm-top
scheme_count: 1
schemes:
- evidence: '所有调用走 {mcp_http} 的 JSON-RPC，请求头携带 Authorization: Bearer {api_key}。'
  header: Authorization
  how_to_obtain: Create a cloud key on the project’s “云端 API” tab; the key is displayed once.
  location: header
  name: api_key
  type: http-bearer
slug: contextlm-top-authentication
source_filename: contextlm-top-authentication.yml
source_heading: Authentication Profile
source_url: https://app.contextlm.top/help/getting-started/overview.md
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://app.contextlm.top/help/getting-started/overview.md\nsources:\n- https://app.contextlm.top/help/getting-started/overview.md\n- https://app.contextlm.top/help/getting-started/quickstart.md\n- https://app.contextlm.top/help/getting-started/chat-vs-project.md\n- https://app.contextlm.top/help/api-access/agent-quickstart.md\ndescription: Authentication schemes for ContextLM API\nschemes:\n- type: http-bearer\n  name: api_key\n  evidence: '所有调用走 {mcp_http} 的 JSON-RPC，请求头携带 Authorization: Bearer {api_key}。'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a cloud key on the project’s “云端 API” tab; the key is displayed once.\ndocs: https://app.contextlm.top/help/getting-started/overview.md\n"
source_yaml_url: https://artifacts.apis.io/contextlm-top/authentication/contextlm-top-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Knowledge Base
- PrivateDocuments
- ContextOS
- CreatorSpace
---
