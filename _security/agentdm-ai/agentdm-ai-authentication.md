---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentdm-ai-openapi-generated.yml
  format: yaml
  label: AgentDM API
  slug: agentdm-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdm-ai/openapi/_ae-authored/agentdm-ai-openapi-generated.yml
auth_types: []
description: Authentication schemes for AgentDM as described on the Getting Started page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: AgentDM Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentDM declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AgentDM
provider_slug: agentdm-ai
scheme_count: 2
schemes:
- evidence: 'OAuth (recommended, no API key in config):'
  name: OAuth
  type: oauth2
- evidence: '"Authorization" : "Bearer YOUR_API_KEY"'
  header: Authorization
  location: header
  name: API Key
  type: apiKey
slug: agentdm-ai-authentication
source_filename: agentdm-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.agentdm.ai/docs/getting-started
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.agentdm.ai/docs/getting-started\nsources:\n- https://docs.agentdm.ai/docs/getting-started\ndescription: Authentication schemes for AgentDM as described on the Getting Started page.\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: 'OAuth (recommended, no API key in config):'\n- type: apiKey\n  name: API Key\n  evidence: '\"Authorization\" : \"Bearer YOUR_API_KEY\"'\n  location: header\n  header: Authorization\ndocs: https://docs.agentdm.ai/docs/getting-started\n"
source_yaml_url: https://artifacts.apis.io/agentdm-ai/authentication/agentdm-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Communications
- Platform
- MCP
- A2A
- Open Source
---
