---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lots-team-openapi-generated.yml
  format: yaml
  label: LotsTeam API
  slug: lots-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lots-team/openapi/_ae-authored/lots-team-openapi-generated.yml
auth_types: []
description: Authentication methods for LotsTeam MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LotsTeam Authentication
name_suffix: Authentication
oauth_flows: []
overview: LotsTeam declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LotsTeam
provider_slug: lots-team
scheme_count: 2
schemes:
- evidence: 'Remote MCP with OAuth: sign in with your LotsTeam account, no key to paste.'
  how_to_obtain: Sign in with the email you use for LotsTeam and allow access.
  name: OAuth
  type: oauth2
- evidence: Agents with HTTP or computer access can use the REST API with an API key.
  how_to_obtain: Obtain an API key from https://www.lotstech.com/api.
  name: API key
  type: apiKey
slug: lots-team-authentication
source_filename: lots-team-authentication.yml
source_heading: Authentication Profile
source_url: https://lots.team/mcp
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lots.team/mcp\nsources:\n- https://lots.team/mcp\n- https://lots.team/agents.md\ndescription: Authentication methods for LotsTeam MCP\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: 'Remote MCP with OAuth: sign in with your LotsTeam account, no key to paste.'\n  how_to_obtain: Sign in with the email you use for LotsTeam and allow access.\n- type: apiKey\n  name: API key\n  evidence: Agents with HTTP or computer access can use the REST API with an API key.\n  how_to_obtain: Obtain an API key from https://www.lotstech.com/api.\ndocs: https://lots.team/mcp\n"
source_yaml_url: https://artifacts.apis.io/lots-team/authentication/lots-team-authentication.yml
summary_line: 2 schemes
tags:
- ProductOps
- Artificial Intelligence
- Feedback
- Software-as-a-Service
- Startups
---
