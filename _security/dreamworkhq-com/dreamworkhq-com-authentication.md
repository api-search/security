---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dreamworkhq-com-openapi-generated.yml
  format: yaml
  label: Dreamwork API
  slug: dreamworkhq-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dreamworkhq-com/openapi/_ae-authored/dreamworkhq-com-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dreamwork Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dreamwork declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dreamwork
provider_slug: dreamworkhq-com
scheme_count: 1
schemes:
- evidence: 'header Copy Authorization: Bearer sk_live_dw_xxxxxxxxxxxxxxxxxxxxxxxx'
  header: Authorization
  how_to_obtain: API keys are created, scoped, and rotated under Profile, then MCP.
  location: header
  name: API Key
  type: http-bearer
slug: dreamworkhq-com-authentication
source_filename: dreamworkhq-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.dreamworkhq.com/agents/docs/authentication
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.dreamworkhq.com/agents/docs/authentication\nsources:\n- https://www.dreamworkhq.com/agents/docs/authentication\n- https://www.dreamworkhq.com/agents/docs/quickstart\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'header Copy Authorization: Bearer sk_live_dw_xxxxxxxxxxxxxxxxxxxxxxxx'\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are created, scoped, and rotated under Profile, then MCP.\nnote: No OAuth2 or other authentication schemes are documented on the provided pages.\ndocs: https://www.dreamworkhq.com/agents/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/dreamworkhq-com/authentication/dreamworkhq-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Job Search
- Automation
- TechCareer
- Platform
---
