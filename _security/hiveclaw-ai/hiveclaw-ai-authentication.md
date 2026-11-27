---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hiveclaw-ai-openapi-generated.yml
  format: yaml
  label: HiveClaw API
  slug: hiveclaw-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hiveclaw-ai/openapi/_ae-authored/hiveclaw-ai-openapi-generated.yml
auth_types: []
description: All HiveClaw API requests are authenticated using API keys sent via the Authorization header as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: HiveClaw Authentication
name_suffix: Authentication
oauth_flows: []
overview: HiveClaw declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: HiveClaw
provider_slug: hiveclaw-ai
scheme_count: 1
schemes:
- evidence: All HiveClaw API requests are authenticated using API keys sent via the Authorization header.
  header: Authorization
  how_to_obtain: Create an API key in the HiveClaw dashboard; the full key is shown once at creation time.
  location: header
  name: Authorization
  type: http-bearer
slug: hiveclaw-ai-authentication
source_filename: hiveclaw-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.hiveclaw.ai/authentication
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.hiveclaw.ai/authentication\nsources:\n- https://docs.hiveclaw.ai/authentication\n- https://docs.hiveclaw.ai/keys\n- https://docs.hiveclaw.ai/quickstart\n- https://docs.hiveclaw.ai/mcp/setup\ndescription: All HiveClaw API requests are authenticated using API keys sent via the Authorization header as a Bearer token.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: All HiveClaw API requests are authenticated using API keys sent via the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the HiveClaw dashboard; the full key is shown once at creation time.\ndocs: https://docs.hiveclaw.ai/authentication\n"
source_yaml_url: https://artifacts.apis.io/hiveclaw-ai/authentication/hiveclaw-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
