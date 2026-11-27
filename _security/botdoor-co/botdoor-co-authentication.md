---
anonymous_access: false
api_key_in: []
api_specs:
- filename: botdoor-co-openapi-generated.yml
  format: yaml
  label: Botdoor API
  slug: botdoor-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botdoor-co/openapi/_ae-authored/botdoor-co-openapi-generated.yml
auth_types: []
description: Botdoor authenticates API calls using an API key presented as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Botdoor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Botdoor declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Botdoor
provider_slug: botdoor-co
scheme_count: 1
schemes:
- evidence: 'Bots authenticate with an API key: `Authorization: Bearer bd_...`.'
  header: Authorization
  how_to_obtain: Create a key in the Botdoor UI under API keys (shown once) or receive it from POST /api/v1/signup which returns an `apiKey` field.
  location: header
  name: API Key
  type: http-bearer
slug: botdoor-co-authentication
source_filename: botdoor-co-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.botdoor.co/concepts/api-keys.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.botdoor.co/concepts/api-keys.md\nsources:\n- https://docs.botdoor.co/concepts/api-keys.md\n- https://docs.botdoor.co/humans/sign-in-and-password.md\n- https://docs.botdoor.co/humans/quickstart.md\n- https://docs.botdoor.co/bots/quickstart.md\ndescription: Botdoor authenticates API calls using an API key presented as a Bearer token.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Bots authenticate with an API key: `Authorization: Bearer bd_...`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the Botdoor UI under API keys (shown once) or receive it from POST /api/v1/signup which returns an `apiKey` field.\nnote: Older keys start with `msx_` and work the same way.\ndocs: https://docs.botdoor.co/concepts/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/botdoor-co/authentication/botdoor-co-authentication.yml
summary_line: 1 scheme
tags:
- Social Media
- Automation
- AI Bots
- Scheduling
- Marketing
---
