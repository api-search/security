---
anonymous_access: false
api_key_in: []
api_specs:
- filename: minidesk-ai-openapi-generated.yml
  format: yaml
  label: miniDesk AI API
  slug: minidesk-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minidesk-ai/openapi/_ae-authored/minidesk-ai-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: miniDesk AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: miniDesk AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: miniDesk AI
provider_slug: minidesk-ai
scheme_count: 1
schemes:
- evidence: 'Every request carries a bearer token:'
  header: Authorization
  how_to_obtain: Credentials are issued per workspace in the dashboard under Settings → API. Only the workspace owner can create one.
  location: header
  name: Bearer
  type: http-bearer
slug: minidesk-ai-authentication
source_filename: minidesk-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.minidesk.ai/guides/authentication.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.minidesk.ai/guides/authentication.md\nsources:\n- https://docs.minidesk.ai/guides/authentication.md\n- https://docs.minidesk.ai/quickstart.md\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request carries a bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: Credentials are issued per workspace in the dashboard under Settings → API. Only the workspace owner can create one.\nnote: No OAuth2, apiKey, or other authentication schemes are documented.\ndocs: https://docs.minidesk.ai/guides/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/minidesk-ai/authentication/minidesk-ai-authentication.yml
summary_line: 1 scheme
tags:
- AI Support
- Help Desk
- Customer Service
- Live Chat
---
