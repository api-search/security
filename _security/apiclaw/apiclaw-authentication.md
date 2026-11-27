---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apiclaw-openapi.json
  format: json
  label: APIClaw
  slug: apiclaw
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiclaw/openapi/_original/apiclaw-openapi.json
auth_types: []
description: APIClaw authenticates requests using an API key passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: APIClaw Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIClaw declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: APIClaw
provider_slug: apiclaw
scheme_count: 1
schemes:
- evidence: 'curl https://apiclaw.biz/v1/chat/completions \ -H "Authorization: Bearer sk-your-apiclaw-key" \ -H "Content-Type: application/json" \ ...'
  header: Authorization
  how_to_obtain: Copy your API key from the APIClaw dashboard.
  location: header
  name: API Key
  type: http-bearer
slug: apiclaw-authentication
source_filename: apiclaw-authentication.yml
source_heading: Authentication Profile
source_url: https://apiclaw.biz/claude-code-api-setup/
source_yaml: "generated: '2026-09-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://apiclaw.biz/claude-code-api-setup/\nsources:\n- https://apiclaw.biz/claude-code-api-setup/\n- https://apiclaw.biz/kilo-code-api-setup/\n- https://apiclaw.biz/blog/cheapest-claude-api/\ndescription: APIClaw authenticates requests using an API key passed as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'curl https://apiclaw.biz/v1/chat/completions \\ -H \"Authorization: Bearer sk-your-apiclaw-key\" \\ -H \"Content-Type: application/json\"\n    \\ ...'\n  location: header\n  header: Authorization\n  how_to_obtain: Copy your API key from the APIClaw dashboard.\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the provided pages.\ndocs: https://apiclaw.biz/claude-code-api-setup/\n"
source_yaml_url: https://artifacts.apis.io/apiclaw/authentication/apiclaw-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- LLM
- Software-as-a-Service
- Platform
---
