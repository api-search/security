---
anonymous_access: true
api_key_in: []
api_specs:
- filename: childadhd-ai-articles-api-openapi.yml
  format: yaml
  label: ADHD in Children Articles API
  slug: childadhd-ai-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/childadhd-ai/openapi/childadhd-ai-articles-api-openapi.yml
- filename: childadhd-ai-mcp-api-openapi.yml
  format: yaml
  label: ADHD in Children MCP API
  slug: childadhd-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/childadhd-ai/openapi/childadhd-ai-mcp-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: ADHD in Children Authentication
name_suffix: Authentication
oauth_flows: []
overview: ADHD in Children declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ADHD in Children
provider_slug: childadhd-ai
scheme_count: 1
schemes:
- description: No authentication. All REST endpoints (/api/v1/articles, /api/v1/articles/search, /api/v1/articles/{slug}) and the MCP endpoint (/api/mcp/v1) are documented as anonymous.
  evidence:
  - https://childadhd.ai/.well-known/api-catalog
  - https://childadhd.ai/.well-known/mcp/server-card.json
  - https://childadhd.ai/openapi.json
  type: none
slug: childadhd-ai-authentication
source_filename: childadhd-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://childadhd.ai/.well-known/api-catalog\ndocs: https://childadhd.ai/llms.txt\nanonymous: true\nnote: 'The OpenAPI document declares no securitySchemes and no security requirement. The provider''s RFC 9727 API catalog lists every service with \"authentication\": \"none\", and the MCP server card declares transport authentication \"none\". The OpenAPI info.description says \"Anonymous, ready to call.\"'\nschemes:\n- type: none\n  description: No authentication. All REST endpoints (/api/v1/articles, /api/v1/articles/search, /api/v1/articles/{slug}) and the MCP endpoint (/api/mcp/v1) are documented as anonymous.\n  evidence:\n  - https://childadhd.ai/.well-known/api-catalog\n  - https://childadhd.ai/.well-known/mcp/server-card.json\n  - https://childadhd.ai/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/childadhd-ai/authentication/childadhd-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- ADHD
- Pediatric Mental Health
- Parenting
- Health Information
- Behavioral Health
- MCP
- content-api
---
