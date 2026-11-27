---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods as described on LooperTask quickstart pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LooperTask Authentication
name_suffix: Authentication
oauth_flows: []
overview: LooperTask declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LooperTask
provider_slug: loopertask-com
scheme_count: 2
schemes:
- evidence: 'Authorization: Bearer tm_YOUR_AGENT_TOKEN'
  header: Authorization
  how_to_obtain: Copy the agent token from Board settings → AI agents (it starts with tm_).
  location: header
  name: Bearer Token
  type: http-bearer
- evidence: Authenticate over OAuth (add LooperTask as a connector in Claude)
  how_to_obtain: Add LooperTask as a connector in Claude to perform OAuth flow.
  name: OAuth
  type: oauth2
slug: loopertask-com-authentication
source_filename: loopertask-com-authentication.yml
source_heading: Authentication Profile
source_url: https://loopertask.com/docs/quickstart
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://loopertask.com/docs/quickstart\nsources:\n- https://loopertask.com/docs/quickstart\n- https://loopertask.com/de/docs/quickstart\n- https://loopertask.com/docs/quickstart?lang=en\ndescription: Authentication methods as described on LooperTask quickstart pages.\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: 'Authorization: Bearer tm_YOUR_AGENT_TOKEN'\n  location: header\n  header: Authorization\n  how_to_obtain: Copy the agent token from Board settings → AI agents (it starts with tm_).\n- type: oauth2\n  name: OAuth\n  evidence: Authenticate over OAuth (add LooperTask as a connector in Claude)\n  how_to_obtain: Add LooperTask as a connector in Claude to perform OAuth flow.\ndocs: https://loopertask.com/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/loopertask-com/authentication/loopertask-com-authentication.yml
summary_line: 2 schemes
tags:
- Time Tracking
- Invoicing
- AI Automation
- Studio
- Agencies
---
