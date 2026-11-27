---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for App Listing Agent
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: App Listing Agent Authentication
name_suffix: Authentication
oauth_flows: []
overview: App Listing Agent declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: App Listing Agent
provider_slug: applistingagent-com
scheme_count: 3
schemes:
- evidence: OAuth — clients that support remote-MCP OAuth open a browser sign-in. You choose one app workspace and the authority the agent gets.
  name: OAuth
  type: oauth2
- evidence: One-time pairing — during onboarding, choose Connect my agent. App Listing Agent shows a single-use code that expires after 15 minutes and a setup prompt to paste into your agent. The agent exchanges the code for a scoped key.
  how_to_obtain: Obtain a single‑use pairing code during onboarding; paste the provided setup prompt into the agent, which exchanges it for a scoped key.
  name: One-time pairing
  type: other
- evidence: Scoped API key — create a key yourself and add it to your MCP client configuration.
  header: Authorization
  how_to_obtain: Create a key in Settings → Agent & API Keys; the key starts with "asc_live_" and is used as a bearer token.
  location: header
  name: Scoped API key
  type: apiKey
slug: applistingagent-com-authentication
source_filename: applistingagent-com-authentication.yml
source_heading: Authentication Profile
source_url: https://applistingagent.com/docs/authentication.md
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://applistingagent.com/docs/authentication.md\nsources:\n- https://applistingagent.com/docs/authentication.md\n- https://applistingagent.com/docs/mcp/installation\n- https://applistingagent.com/docs/authentication\n- https://applistingagent.com/docs/getting-started.md\ndescription: Authentication methods for App Listing Agent\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: OAuth — clients that support remote-MCP OAuth open a browser sign-in. You choose one app workspace and the authority the agent gets.\n- type: other\n  name: One-time pairing\n  evidence: One-time pairing — during onboarding, choose Connect my agent. App Listing Agent shows a single-use code that expires after 15 minutes\n    and a setup prompt to paste into your agent. The agent exchanges the code for a scoped key.\n  how_to_obtain: Obtain a single‑use pairing code during onboarding; paste the provided\
  \ setup prompt into the agent, which exchanges it for a\n    scoped key.\n- type: apiKey\n  name: Scoped API key\n  evidence: Scoped API key — create a key yourself and add it to your MCP client configuration.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Settings → Agent & API Keys; the key starts with \"asc_live_\" and is used as a bearer token.\ndocs: https://applistingagent.com/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/applistingagent-com/authentication/applistingagent-com-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- App Store
- Automation
- Software-as-a-Service
- Marketing
---
