---
api_key_in: []
api_specs:
- filename: signal-ai-openapi-original.json
  format: json
  label: Signal AI API
  slug: signal-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Signal Ai Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Signal AI secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Signal AI
provider_slug: signal-ai
scheme_count: 1
schemes:
- description: "To obtain the Bearer Token using the Client ID / Secret pair provided to you:\n\n```bash\ncurl -X POST \\\n  -d 'grant_type=client_credentials' \\\n  -d 'client_id=YOUR_CLIENT_ID' \\\n  -d 'client_secret=YOUR_CLIENT_SECRET' \\\n  https://api.signal-ai.com/auth/token\n```\n\nThis will return the following JSON response:\n\n```json\n{\n    \"access_token\": \"eyJhbGciOi…\",\n    \"expires_in\": 86400,\n    …\n}\n```\n\nYou must "
  flows:
  - flow: clientCredentials
    scopes: 6
    tokenUrl: https://api.signal-ai.com/auth/token
  name: OAuth2
  sources:
  - openapi/signal-ai-openapi-original.json
  type: oauth2
slug: signal-ai-authentication
source_filename: signal-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/signal-ai-openapi-original.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.signal-ai.com/auth/token\n    scopes: 6\n  description: \"To obtain the Bearer Token using the Client ID / Secret pair provided to you:\\n\\\n    \\n```bash\\ncurl -X POST \\\\\\n  -d 'grant_type=client_credentials' \\\\\\n  -d 'client_id=YOUR_CLIENT_ID'\\\n    \\ \\\\\\n  -d 'client_secret=YOUR_CLIENT_SECRET' \\\\\\n  https://api.signal-ai.com/auth/token\\n\\\n    ```\\n\\nThis will return the following JSON response:\\n\\n```json\\n{\\n    \\\"access_token\\\"\\\n    : \\\"eyJhbGciOi…\\\",\\n    \\\"expires_in\\\": 86400,\\n    …\\n}\\n```\\n\\nYou must \"\n  sources:\n  - openapi/signal-ai-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/authentication/signal-ai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Media Intelligence
- Reputation Management
- Risk Intelligence
- News
- Content Search
- Knowledge Graph
- ESG
- Artificial Intelligence
- Analytics
---
