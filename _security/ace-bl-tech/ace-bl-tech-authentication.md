---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ace-bl-tech-agent-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Agent API
  slug: ace-bl-tech-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-agent-api-openapi.yml
- filename: ace-bl-tech-apps-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Apps API
  slug: ace-bl-tech-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-apps-api-openapi.yml
- filename: ace-bl-tech-catalog-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Catalog API
  slug: ace-bl-tech-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-catalog-api-openapi.yml
- filename: ace-bl-tech-connections-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Connections API
  slug: ace-bl-tech-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-connections-api-openapi.yml
- filename: ace-bl-tech-custom-connectors-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Custom Connectors API
  slug: ace-bl-tech-custom-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-custom-connectors-api-openapi.yml
- filename: ace-bl-tech-events-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Events API
  slug: ace-bl-tech-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-events-api-openapi.yml
- filename: ace-bl-tech-mcp-api-openapi.yml
  format: yaml
  label: Ace AI Assistant MCP API
  slug: ace-bl-tech-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-mcp-api-openapi.yml
- filename: ace-bl-tech-me-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Me API
  slug: ace-bl-tech-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-me-api-openapi.yml
- filename: ace-bl-tech-runs-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Runs API
  slug: ace-bl-tech-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-runs-api-openapi.yml
- filename: ace-bl-tech-tools-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Tools API
  slug: ace-bl-tech-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-tools-api-openapi.yml
- filename: ace-bl-tech-triggers-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Triggers API
  slug: ace-bl-tech-triggers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-triggers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ace Bl Tech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ace AI Assistant secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ace AI Assistant
provider_slug: ace-bl-tech
scheme_count: 1
schemes:
- bearerFormat: ace_sk_…
  description: 'An Ace API key from https://tryacee.com/developers. x-api-key: <key> also works.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/tryacee.com-openapi.json
  type: http
slug: ace-bl-tech-authentication
source_filename: ace-bl-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/tryacee.com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: ace_sk_…\n  description: 'An Ace API key from https://tryacee.com/developers. x-api-key: <key> also works.'\n  sources:\n  - openapi/tryacee.com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/ace-bl-tech/authentication/ace-bl-tech-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Productivity
- Assistant
- macOS
- Windows
- iOS
---
