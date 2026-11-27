---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CodeMind Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodeMind secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CodeMind
provider_slug: codemindhq-dev
scheme_count: 1
schemes:
- applies_to:
  - https://api.codemindhq.dev/builds
  - https://api.codemindhq.dev/mcp
  description: 'Every documented example sends "Authorization: Bearer $CODEMIND_API_KEY", for both the REST API (POST https://api.codemindhq.dev/builds) and the remote MCP server (https://api.codemindhq.dev/mcp, via the MCP client headers config).'
  name: bearerApiKey
  scheme: bearer
  type: http
slug: codemindhq-dev-authentication
source_filename: codemindhq-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://codemindhq.dev/\ndocs: https://codemindhq.dev/\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  description: 'Every documented example sends \"Authorization: Bearer $CODEMIND_API_KEY\", for both the REST API (POST https://api.codemindhq.dev/builds) and the remote MCP server (https://api.codemindhq.dev/mcp, via the MCP client headers config).'\n  applies_to:\n  - https://api.codemindhq.dev/builds\n  - https://api.codemindhq.dev/mcp\nnote: No OpenAPI is published, so this is read from the homepage examples. The site does not document how keys are issued, scoped or rotated; its Sign in / Start free links are '#' placeholders.\n"
source_yaml_url: https://artifacts.apis.io/codemindhq-dev/authentication/codemindhq-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI Coding
- Code Generation
- MCP
- Developer Tools
- GitHub
- Pull Requests
- Code Verification
---
