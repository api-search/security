---
anonymous_access: false
api_key_in: []
api_specs:
- filename: waterr-ai-api-openapi.yml
  format: yaml
  label: WaterrAI API API
  slug: waterrai-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/waterr-ai/openapi/_original/waterr-ai-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Waterr Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: waterr-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: waterr-ai
provider_slug: waterr-ai
scheme_count: 1
schemes:
- evidence: 'Send the key in the `Authorization` header on any API request:'
  header: Authorization
  how_to_obtain: Create an API key in the WaterrAI dashboard (Settings → API Keys) and copy the shown `wai_` prefixed key.
  location: header
  name: API Key
  type: http-bearer
slug: waterr-ai-authentication
source_filename: waterr-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.waterr.ai/api-reference/authentication.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.waterr.ai/api-reference/authentication.md\nsources:\n- https://docs.waterr.ai/api-reference/authentication.md\n- https://docs.waterr.ai/customization/personalization-tokens.md\n- https://docs.waterr.ai/api-reference/embed-tokens.md\n- https://docs.waterr.ai/getting-started/core-concepts.md\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Send the key in the `Authorization` header on any API request:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the WaterrAI dashboard (Settings → API Keys) and copy the shown `wai_` prefixed key.\ndocs: https://docs.waterr.ai/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/waterr-ai/authentication/waterr-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Meetings
- Video
- Automation
---
