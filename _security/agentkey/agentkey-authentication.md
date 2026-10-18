---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentkey-install-api-openapi.yml
  format: yaml
  label: AgentKey (Data API Layer) Install API
  slug: agentkey-install-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentkey/refs/heads/main/openapi/agentkey-install-api-openapi.yml
auth_types: []
description: Authentication schemes for AgentKey
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agentkey Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentKey (Data API Layer) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AgentKey (Data API Layer)
provider_slug: agentkey
scheme_count: 1
schemes:
- evidence: AgentKey authenticates with a single **master key**.
  how_to_obtain: Generate a key in the console.
  name: master key
  type: apiKey
slug: agentkey-authentication
source_filename: agentkey-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.agentkey.app/authentication.md
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.agentkey.app/authentication.md\nsources:\n- https://docs.agentkey.app/authentication.md\n- https://docs.agentkey.app/quickstart.md\ndescription: Authentication schemes for AgentKey\nschemes:\n- type: apiKey\n  name: master key\n  evidence: AgentKey authenticates with a single **master key**.\n  how_to_obtain: Generate a key in the console.\nnote: No OAuth flows or other authentication types are documented.\ndocs: https://docs.agentkey.app/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentkey/refs/heads/main/authentication/agentkey-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data
- Integration
- Artificial Intelligence
- Automation
---
