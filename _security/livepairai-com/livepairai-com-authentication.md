---
anonymous_access: false
api_key_in: []
api_specs:
- filename: livepairai-com-agent-api-openapi.yml
  format: yaml
  label: LivePair AI Agent API
  slug: livepairai-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livepairai-com/openapi/livepairai-com-agent-api-openapi.yml
auth_types: []
description: LivePair AI uses API keys for authentication.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LivePair AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: LivePair AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LivePair AI
provider_slug: livepairai-com
scheme_count: 2
schemes:
- evidence: 'Send it as x-api-key: lp_… or Authorization: Bearer lp_….'
  header: x-api-key
  how_to_obtain: 'Create/manage: Settings → API keys'
  location: header
  name: x-api-key
  type: apiKey
- evidence: 'Send it as x-api-key: lp_… or Authorization: Bearer lp_….'
  header: Authorization
  how_to_obtain: 'Create/manage: Settings → API keys'
  location: header
  name: Bearer
  type: http-bearer
slug: livepairai-com-authentication
source_filename: livepairai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://livepairai.com/docs/api-keys
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://livepairai.com/docs/api-keys\nsources:\n- https://livepairai.com/docs/api-keys\n- https://livepairai.com/token\n- https://livepairai.com/blog/gpt-6-astra-api\n- https://livepairai.com/blog/grok-4-7-api\ndescription: LivePair AI uses API keys for authentication.\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: 'Send it as x-api-key: lp_… or Authorization: Bearer lp_….'\n  location: header\n  header: x-api-key\n  how_to_obtain: 'Create/manage: Settings → API keys'\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send it as x-api-key: lp_… or Authorization: Bearer lp_….'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Create/manage: Settings → API keys'\nnote: No OAuth2, JWT, HMAC, MTLS, or other authentication schemes are documented.\ndocs: https://livepairai.com/docs/api-keys\n"
source_yaml_url: https://artifacts.apis.io/livepairai-com/authentication/livepairai-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Image Generation
- Video Generation
- Private API
- Community
---
