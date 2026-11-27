---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: BacklinkGenie Authentication
name_suffix: Authentication
oauth_flows: []
overview: BacklinkGenie declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BacklinkGenie
provider_slug: backlinkgenie-com
scheme_count: 2
schemes:
- auth_url: https://app.backlinkgenie.com/oauth/authorize
  description: OAuth 2.1 with dynamic client registration, used by Claude, ChatGPT, Cursor integrations.
  flow: authorization_code
  token_url: https://app.backlinkgenie.com/oauth/token
  type: oauth2
- description: Bearer token (bg_live_...) generated in Settings → MCP for script/CI usage.
  in: header
  name: Authorization
  type: apiKey
slug: backlinkgenie-com-authentication
source_filename: backlinkgenie-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://backlinkgenie.com/llms.txt\nschemes:\n  - type: oauth2\n    flow: authorization_code\n    description: \"OAuth 2.1 with dynamic client registration, used by Claude, ChatGPT, Cursor integrations.\"\n    auth_url: \"https://app.backlinkgenie.com/oauth/authorize\"\n    token_url: \"https://app.backlinkgenie.com/oauth/token\"\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Bearer token (bg_live_...) generated in Settings → MCP for script/CI usage.\"\n"
source_yaml_url: https://artifacts.apis.io/backlinkgenie-com/authentication/backlinkgenie-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- SEO
- Link Building
- Marketing
- Automation
---
