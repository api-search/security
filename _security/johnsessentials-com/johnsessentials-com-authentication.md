---
anonymous_access: false
api_key_in: []
api_specs:
- filename: johnsessentials-com-agent-api-openapi.yml
  format: yaml
  label: John\'s Essentials Agent API
  slug: johnsessentials-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/johnsessentials-com/openapi/johnsessentials-com-agent-api-openapi.yml
- filename: johnsessentials-com-authentication-api-openapi.yml
  format: yaml
  label: John\'s Essentials Authentication API
  slug: johnsessentials-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/johnsessentials-com/openapi/johnsessentials-com-authentication-api-openapi.yml
- filename: johnsessentials-com-files-api-openapi.yml
  format: yaml
  label: John\'s Essentials Files API
  slug: johnsessentials-com-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/johnsessentials-com/openapi/johnsessentials-com-files-api-openapi.yml
- filename: johnsessentials-com-mcp-api-openapi.yml
  format: yaml
  label: John\'s Essentials MCP API
  slug: johnsessentials-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/johnsessentials-com/openapi/johnsessentials-com-mcp-api-openapi.yml
- filename: johnsessentials-com-memory-api-openapi.yml
  format: yaml
  label: John\'s Essentials Memory API
  slug: johnsessentials-com-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/johnsessentials-com/openapi/johnsessentials-com-memory-api-openapi.yml
- filename: johnsessentials-com-openai-compatibility-api-openapi.yml
  format: yaml
  label: John\'s Essentials OpenAI Compatibility API
  slug: johnsessentials-com-openai-compatibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/johnsessentials-com/openapi/johnsessentials-com-openai-compatibility-api-openapi.yml
- filename: johnsessentials-com-organizations-api-openapi.yml
  format: yaml
  label: John\'s Essentials Organizations API
  slug: johnsessentials-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/johnsessentials-com/openapi/johnsessentials-com-organizations-api-openapi.yml
- filename: johnsessentials-com-status-api-openapi.yml
  format: yaml
  label: John\'s Essentials Status API
  slug: johnsessentials-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/johnsessentials-com/openapi/johnsessentials-com-status-api-openapi.yml
- filename: johnsessentials-com-tools-api-openapi.yml
  format: yaml
  label: John\'s Essentials Tools API
  slug: johnsessentials-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/johnsessentials-com/openapi/johnsessentials-com-tools-api-openapi.yml
- filename: johnsessentials-com-webhooks-api-openapi.yml
  format: yaml
  label: John\'s Essentials Webhooks API
  slug: johnsessentials-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/johnsessentials-com/openapi/johnsessentials-com-webhooks-api-openapi.yml
- filename: johnsessentials-com-workflows-api-openapi.yml
  format: yaml
  label: John\'s Essentials Workflows API
  slug: johnsessentials-com-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/johnsessentials-com/openapi/johnsessentials-com-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: John\'s Essentials Authentication
name_suffix: Authentication
oauth_flows: []
overview: John\'s Essentials secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: John\'s Essentials
provider_slug: johnsessentials-com
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: 'Bearer token = your API key, prefixed `je_live_sk_`.

    Example: `Authorization: Bearer je_live_sk_abc123...`'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/johnsessentials-com-openapi.json
  type: http
slug: johnsessentials-com-authentication
source_filename: johnsessentials-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/johnsessentials-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: |-\n    Bearer token = your API key, prefixed `je_live_sk_`.\n    Example: `Authorization: Bearer je_live_sk_abc123...`\n  sources:\n  - openapi/johnsessentials-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/johnsessentials-com/authentication/johnsessentials-com-authentication.yml
summary_line: http · 1 scheme
tags:
- File Processing
- AI Tools
- Automation
- Document Management
- Media Conversion
---
