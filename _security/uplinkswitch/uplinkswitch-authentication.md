---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for UplinkSwitch API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Uplinkswitch Authentication
name_suffix: Authentication
oauth_flows: []
overview: UplinkSwitch declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: UplinkSwitch
provider_slug: uplinkswitch
scheme_count: 2
schemes:
- evidence: 'curl https://api.uplinkswitch.com/v1/models -H "Authorization: Bearer $UPLINKSWITCH_API_KEY"'
  header: Authorization
  how_to_obtain: Create a key in the UplinkSwitch console; the key is shown once and can be used as a bearer token.
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'curl https://api.uplinkswitch.com/v1/models -H "x-api-key: $ANTHROPIC_API_KEY"'
  header: x-api-key
  how_to_obtain: Create a key in the UplinkSwitch console; the key is shown once and can be sent in the x-api-key header.
  location: header
  name: x-api-key
  type: other
slug: uplinkswitch-authentication
source_filename: uplinkswitch-authentication.yml
source_heading: Authentication Profile
source_url: https://uplinkswitch.ai/guides/kilo-code
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://uplinkswitch.ai/guides/kilo-code\nsources:\n- https://uplinkswitch.ai/guides/kilo-code\n- https://uplinkswitch.ai/blog/best-uncensored-llm\n- https://uplinkswitch.ai/blog/claude-api-key\n- https://uplinkswitch.ai/blog/cursor-api-key-cost\ndescription: Authentication methods for UplinkSwitch API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'curl https://api.uplinkswitch.com/v1/models -H \"Authorization: Bearer $UPLINKSWITCH_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the UplinkSwitch console; the key is shown once and can be used as a bearer token.\n- type: other\n  name: x-api-key\n  evidence: 'curl https://api.uplinkswitch.com/v1/models -H \"x-api-key: $ANTHROPIC_API_KEY\"'\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a key in the UplinkSwitch console; the key is shown once and can\
  \ be sent in the x-api-key header.\ndocs: https://uplinkswitch.ai/guides/kilo-code\n"
source_yaml_url: https://artifacts.apis.io/uplinkswitch/authentication/uplinkswitch-authentication.yml
summary_line: 2 schemes
tags:
- AI
- LLM
- Gateway
- Reseller
- Platform
---
