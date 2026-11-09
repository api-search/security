---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for AgentPlaybooks APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Agentplaybooks Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentPlaybooks declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AgentPlaybooks
provider_slug: agentplaybooks-ai
scheme_count: 2
schemes:
- evidence: Go to the API Keys tab Click "Generate New Key"
  header: Authorization
  how_to_obtain: Generate a new key in the API Keys tab of the AgentPlaybooks dashboard
  location: header
  name: API Key
  type: http-bearer
- evidence: OAuth redirect URLs must be configured in the Supabase Dashboard , not in code.
  how_to_obtain: Configure OAuth providers (GitHub, Google, LinkedIn) in Supabase Dashboard and obtain client credentials there
  name: Supabase OAuth
  type: oauth2
slug: agentplaybooks-ai-authentication
source_filename: agentplaybooks-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://agentplaybooks.ai/docs/hermes-portable-agents
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agentplaybooks.ai/docs/hermes-portable-agents\nsources:\n- https://agentplaybooks.ai/docs/hermes-portable-agents\n- https://agentplaybooks.ai/docs/getting-started.md\n- https://agentplaybooks.ai/docs/getting-started\n- https://agentplaybooks.ai/docs/environment-setup\ndescription: Authentication methods for AgentPlaybooks APIs\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Go to the API Keys tab Click \"Generate New Key\"\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a new key in the API Keys tab of the AgentPlaybooks dashboard\n- type: oauth2\n  name: Supabase OAuth\n  evidence: OAuth redirect URLs must be configured in the Supabase Dashboard , not in code.\n  how_to_obtain: Configure OAuth providers (GitHub, Google, LinkedIn) in Supabase Dashboard and obtain client credentials there\ndocs: https://agentplaybooks.ai/docs/hermes-portable-agents\n"
source_yaml_url: https://artifacts.apis.io/agentplaybooks-ai/authentication/agentplaybooks-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Playbooks
- Documentation
- Open Source
---
