---
anonymous_access: false
api_key_in: []
api_specs:
- filename: limy-ai-openapi-generated.yml
  format: yaml
  label: Limy AI API
  slug: limy-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/limy-ai/openapi/_ae-authored/limy-ai-openapi-generated.yml
auth_types: []
description: Authentication schemes for Limy AI REST API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Limy AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Limy AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Limy AI
provider_slug: limy-ai
scheme_count: 1
schemes:
- evidence: Send your static API key as a Bearer token. Returns a short-lived session JWT to use on all subsequent API requests.
  header: Authorization
  how_to_obtain: Generate an API key via the Limy Admin Dashboard (see Create an API key page).
  location: header
  name: bearer
  type: http-bearer
slug: limy-ai-authentication
source_filename: limy-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.getlimy.ai/rest-api/api-reference/authentication.md
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.getlimy.ai/rest-api/api-reference/authentication.md\nsources:\n- https://docs.getlimy.ai/rest-api/api-reference/authentication.md\n- https://docs.getlimy.ai/rest-api/create-an-api-key.md\n- https://docs.getlimy.ai/rest-api/authentication.md\n- https://limy.ai/blog/chatgpt-didn-t-stop-sending-traffic.-it-stopped-signing-it\ndescription: Authentication schemes for Limy AI REST API\nschemes:\n- type: http-bearer\n  name: bearer\n  evidence: Send your static API key as a Bearer token. Returns a short-lived session JWT to use on all subsequent API requests.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key via the Limy Admin Dashboard (see Create an API key page).\nnote: No OAuth2, apiKey, or other authentication schemes are documented.\ndocs: https://docs.getlimy.ai/rest-api/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/limy-ai/authentication/limy-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Marketing
- Analytics
- Competitive Intelligence
- Platform
---
