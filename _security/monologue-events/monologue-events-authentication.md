---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Monologue
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Monologue Authentication
name_suffix: Authentication
oauth_flows: []
overview: Monologue declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Monologue
provider_slug: monologue-events
scheme_count: 1
schemes:
- evidence: For a self‑hosted instance, preserve the configured `MONOLOGUE_URL` and `MONOLOGUE_API_KEY` pairing.
  how_to_obtain: Create an API key at `https://www.monologue.events/keys` and store it in the agent's secret store as `MONOLOGUE_API_KEY`.
  name: Monologue API Key
  type: apiKey
slug: monologue-events-authentication
source_filename: monologue-events-authentication.yml
source_heading: Authentication Profile
source_url: https://www.monologue.events/agent-setup
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.monologue.events/agent-setup\nsources:\n- https://www.monologue.events/agent-setup\n- https://www.monologue.events/agent-setup/SKILL.md\ndescription: Authentication methods for Monologue\nschemes:\n- type: apiKey\n  name: Monologue API Key\n  evidence: For a self‑hosted instance, preserve the configured `MONOLOGUE_URL` and `MONOLOGUE_API_KEY` pairing.\n  how_to_obtain: Create an API key at `https://www.monologue.events/keys` and store it in the agent's secret store as `MONOLOGUE_API_KEY`.\ndocs: https://www.monologue.events/agent-setup\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/monologue-events/authentication/monologue-events-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Feed
- Privacy
- Monitoring
- Automation
---
