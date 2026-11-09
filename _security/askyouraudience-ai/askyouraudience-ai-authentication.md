---
anonymous_access: false
api_key_in: []
api_specs:
- filename: askyouraudience-ai-openapi-generated.yml
  format: yaml
  label: Ask Your Audience API
  slug: askyouraudience-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/askyouraudience-ai/openapi/_ae-authored/askyouraudience-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for Ask Your Audience API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Askyouraudience Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ask Your Audience declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ask Your Audience
provider_slug: askyouraudience-ai
scheme_count: 2
schemes:
- evidence: 'http Authorization: Bearer <oauth-access-token>'
  header: Authorization
  location: header
  name: OAuth
  type: http-bearer
- evidence: 'X-Api-Key: aya_test_...'
  header: X-Api-Key
  location: header
  name: Workspace API Key
  type: apiKey
slug: askyouraudience-ai-authentication
source_filename: askyouraudience-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.askyouraudience.ai/docs/auth
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.askyouraudience.ai/docs/auth\nsources:\n- https://www.askyouraudience.ai/docs/auth\n- https://developers.askyouraudience.ai/docs/auth\n- https://www.askyouraudience.ai/docs\ndescription: Authentication methods for Ask Your Audience API\nschemes:\n- type: http-bearer\n  name: OAuth\n  evidence: 'http Authorization: Bearer <oauth-access-token>'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: Workspace API Key\n  evidence: 'X-Api-Key: aya_test_...'\n  location: header\n  header: X-Api-Key\ndocs: https://www.askyouraudience.ai/docs/auth\n"
source_yaml_url: https://artifacts.apis.io/askyouraudience-ai/authentication/askyouraudience-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- AudienceResearch
- MarketTesting
- Digital Twin
---
