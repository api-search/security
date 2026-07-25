---
api_key_in: []
api_specs:
- filename: smithery-ai-connect-api-openapi.yml
  format: yaml
  label: Smithery connect API
  slug: smithery-ai-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-connect-api-openapi.yml
- filename: smithery-ai-connect-mcp-api-openapi.yml
  format: yaml
  label: Smithery connect.mcp API
  slug: smithery-ai-connect-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-connect-mcp-api-openapi.yml
- filename: smithery-ai-domains-api-openapi.yml
  format: yaml
  label: Smithery domains API
  slug: smithery-ai-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-domains-api-openapi.yml
- filename: smithery-ai-health-api-openapi.yml
  format: yaml
  label: Smithery Health API
  slug: smithery-ai-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-health-api-openapi.yml
- filename: smithery-ai-namespaces-api-openapi.yml
  format: yaml
  label: Smithery namespaces API
  slug: smithery-ai-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-namespaces-api-openapi.yml
- filename: smithery-ai-organizations-api-openapi.yml
  format: yaml
  label: Smithery organizations API
  slug: smithery-ai-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-organizations-api-openapi.yml
- filename: smithery-ai-servers-api-openapi.yml
  format: yaml
  label: Smithery servers API
  slug: smithery-ai-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-servers-api-openapi.yml
- filename: smithery-ai-skills-api-openapi.yml
  format: yaml
  label: Smithery skills API
  slug: smithery-ai-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-skills-api-openapi.yml
- filename: smithery-ai-tokens-api-openapi.yml
  format: yaml
  label: Smithery tokens API
  slug: smithery-ai-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-tokens-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Smithery Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smithery secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smithery
provider_slug: smithery-ai
scheme_count: 1
schemes:
- description: Smithery API key as Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/smithery-connect-api-openapi.yml
  - openapi/smithery-registry-api-openapi.yml
  type: http
slug: smithery-ai-authentication
source_filename: smithery-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smithery-connect-api-openapi.yml, openapi/smithery-registry-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Smithery API key as Bearer token\n  sources:\n  - openapi/smithery-connect-api-openapi.yml\n  - openapi/smithery-registry-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/authentication/smithery-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Agents
- MCP
- Model Context Protocol
- Registry
- Hosting
- Tools
- Skills
- Marketplace
- Developer Platform
---
