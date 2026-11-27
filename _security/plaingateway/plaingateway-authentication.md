---
anonymous_access: false
api_key_in: []
api_specs:
- filename: plaingateway-chat-completions-api-openapi.yml
  format: yaml
  label: plaingateway Chat Completions API
  slug: plaingateway-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaingateway/openapi/plaingateway-chat-completions-api-openapi.yml
auth_types: []
description: Authentication via API key
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: plaingateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: plaingateway declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: plaingateway
provider_slug: plaingateway
scheme_count: 2
schemes:
- evidence: 'Send it as `Authorization: Bearer sk-pg-v1-...`, or as `X-Api-Key`.'
  header: Authorization
  how_to_obtain: Create a key in the dashboard at /settings/keys and copy the shown key.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'Send it as `Authorization: Bearer sk-pg-v1-...`, or as `X-Api-Key`.'
  header: X-Api-Key
  how_to_obtain: Create a key in the dashboard at /settings/keys and copy the shown key.
  location: header
  name: X-Api-Key header
  type: apiKey
slug: plaingateway-authentication
source_filename: plaingateway-authentication.yml
source_heading: Authentication Profile
source_url: https://plaingateway.com/docs/api/api-keys.md
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://plaingateway.com/docs/api/api-keys.md\nsources:\n- https://plaingateway.com/docs/api/api-keys.md\n- https://plaingateway.com/docs/auth/api-keys.md\n- https://plaingateway.com/docs/api/api-keys\n- https://plaingateway.com/docs/auth/api-keys\ndescription: Authentication via API key\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Send it as `Authorization: Bearer sk-pg-v1-...`, or as `X-Api-Key`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the dashboard at /settings/keys and copy the shown key.\n- type: apiKey\n  name: X-Api-Key header\n  evidence: 'Send it as `Authorization: Bearer sk-pg-v1-...`, or as `X-Api-Key`.'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Create a key in the dashboard at /settings/keys and copy the shown key.\ndocs: https://plaingateway.com/docs/api/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/plaingateway/authentication/plaingateway-authentication.yml
summary_line: 2 schemes
tags:
- Company
- LLM
- API Gateway
- OpenRouter-Alternative
- Free
---
