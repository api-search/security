---
anonymous_access: false
api_key_in: []
auth_types: []
description: FlowStudio MCP uses an API key for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FlowStudio Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlowStudio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FlowStudio
provider_slug: flowstudio-app
scheme_count: 1
schemes:
- evidence: Authentication = API key, Type = Header, Header name = x-api-key
  header: x-api-key
  how_to_obtain: Copy the API key from the dashboard after connecting Power Platform permissions.
  location: header
  name: API key
  type: apiKey
slug: flowstudio-app-authentication
source_filename: flowstudio-app-authentication.yml
source_heading: Authentication Profile
source_url: https://learn.flowstudio.app/blog/create-user-onboarding-workflow-with-power-automate
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://learn.flowstudio.app/blog/create-user-onboarding-workflow-with-power-automate\nsources:\n- https://learn.flowstudio.app/blog/create-user-onboarding-workflow-with-power-automate\n- https://learn.flowstudio.app/mcp-getting-started\n- https://learn.flowstudio.app/getting-started\n- https://learn.flowstudio.app/mcp-cowork-setup\ndescription: FlowStudio MCP uses an API key for authentication.\nschemes:\n- type: apiKey\n  name: API key\n  evidence: Authentication = API key, Type = Header, Header name = x-api-key\n  location: header\n  header: x-api-key\n  how_to_obtain: Copy the API key from the dashboard after connecting Power Platform permissions.\ndocs: https://learn.flowstudio.app/blog/create-user-onboarding-workflow-with-power-automate\n"
source_yaml_url: https://artifacts.apis.io/flowstudio-app/authentication/flowstudio-app-authentication.yml
summary_line: 1 scheme
tags:
- Automation
- Artificial Intelligence
- Power Platform
- Consulting
- Monitoring
---
