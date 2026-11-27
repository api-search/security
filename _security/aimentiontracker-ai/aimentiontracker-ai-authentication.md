---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aimentiontracker-ai-openapi-generated.yml
  format: yaml
  label: aimentiontracker-ai API
  slug: aimentiontracker-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aimentiontracker-ai/openapi/_ae-authored/aimentiontracker-ai-openapi-generated.yml
auth_types: []
description: API key authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: aimentiontracker-ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: aimentiontracker-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: aimentiontracker-ai
provider_slug: aimentiontracker-ai
scheme_count: 1
schemes:
- evidence: 'curl -H "X-API-Key: $RANKHOUND_API_KEY" https://app.rankhound.ai/api/v1/me'
  header: X-API-Key
  how_to_obtain: Mint a key in the RankHound app under API keys (Owner or Admin role).
  location: header
  name: X-API-Key
  type: apiKey
slug: aimentiontracker-ai-authentication
source_filename: aimentiontracker-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://rankhound.ai/docs/quickstart
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://rankhound.ai/docs/quickstart\nsources:\n- https://rankhound.ai/docs/quickstart\ndescription: API key authentication\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'curl -H \"X-API-Key: $RANKHOUND_API_KEY\" https://app.rankhound.ai/api/v1/me'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Mint a key in the RankHound app under API keys (Owner or Admin role).\nnote: No other authentication methods (OAuth, http‑basic, etc.) are documented on the page.\ndocs: https://rankhound.ai/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/aimentiontracker-ai/authentication/aimentiontracker-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- SEO
- Automation
- Marketing
---
