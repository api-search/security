---
anonymous_access: false
api_key_in: []
api_specs:
- filename: keeperhub-com-chains-api-openapi.yml
  format: yaml
  label: KeeperHub Chains API
  slug: keeperhub-com-chains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keeperhub-com/openapi/keeperhub-com-chains-api-openapi.yml
- filename: keeperhub-com-health-api-openapi.yml
  format: yaml
  label: KeeperHub Health API
  slug: keeperhub-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keeperhub-com/openapi/keeperhub-com-health-api-openapi.yml
- filename: keeperhub-com-keys-api-openapi.yml
  format: yaml
  label: KeeperHub Keys API
  slug: keeperhub-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keeperhub-com/openapi/keeperhub-com-keys-api-openapi.yml
- filename: keeperhub-com-mcp-api-openapi.yml
  format: yaml
  label: KeeperHub MCP API
  slug: keeperhub-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keeperhub-com/openapi/keeperhub-com-mcp-api-openapi.yml
auth_types: []
description: Authentication methods for KeeperHub
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: KeeperHub Authentication
name_suffix: Authentication
oauth_flows: []
overview: KeeperHub declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: KeeperHub
provider_slug: keeperhub-com
scheme_count: 2
schemes:
- evidence: Organization keys start with kh_ and authenticate REST and MCP.
  header: Authorization
  how_to_obtain: Create a key in the app under your avatar → API Keys → Organisation tab; keys start with kh_
  name: API Key
  type: http-bearer
- evidence: Run /mcp to complete OAuth in your browser. That mints a short-lived Bearer access token, which is the right credential for an interactive agent.
  header: Authorization
  how_to_obtain: Execute the /mcp endpoint which opens a browser for OAuth flow and returns a short‑lived Bearer token
  name: OAuth
  type: oauth2
slug: keeperhub-com-authentication
source_filename: keeperhub-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.keeperhub.com/getting-started
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.keeperhub.com/getting-started\nsources:\n- https://docs.keeperhub.com/getting-started\n- https://docs.keeperhub.com/getting-started/browser\n- https://docs.keeperhub.com/getting-started/agent\n- https://docs.keeperhub.com/getting-started/api\ndescription: Authentication methods for KeeperHub\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Organization keys start with kh_ and authenticate REST and MCP.\n  header: Authorization\n  how_to_obtain: Create a key in the app under your avatar → API Keys → Organisation tab; keys start with kh_\n- type: oauth2\n  name: OAuth\n  evidence: Run /mcp to complete OAuth in your browser. That mints a short-lived Bearer access token, which is the right credential for an interactive\n    agent.\n  header: Authorization\n  how_to_obtain: Execute the /mcp endpoint which opens a browser for OAuth flow and returns a short‑lived\
  \ Bearer token\ndocs: https://docs.keeperhub.com/getting-started\n"
source_yaml_url: https://artifacts.apis.io/keeperhub-com/authentication/keeperhub-com-authentication.yml
summary_line: 2 schemes
tags:
- Blockchain
- Artificial Intelligence
- Automation
- DeFi
- Onchain
- Company
---
