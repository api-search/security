---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hookbridge-api-openapi.yml
  format: yaml
  label: HookBridge API API
  slug: hookbridge-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookbridge/refs/heads/main/openapi/_original/hookbridge-api-openapi.yml
auth_types: []
description: Authentication schemes for Hookbridge as documented.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hookbridge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hookbridge declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hookbridge
provider_slug: hookbridge
scheme_count: 1
schemes:
- evidence: API keys authenticate requests to the HookBridge API.
  header: Authorization
  how_to_obtain: Create an API key via the HookBridge console or API and copy the key; use it as a Bearer token in the Authorization header.
  location: header
  name: Bearer
  type: http-bearer
slug: hookbridge-authentication
source_filename: hookbridge-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.hookbridge.io/guides/product/api-keys/
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.hookbridge.io/guides/product/api-keys/\nsources:\n- https://docs.hookbridge.io/guides/product/api-keys/\n- https://docs.hookbridge.io/guides/product/api-keys\n- https://docs.hookbridge.io/api/operations/tags/api-keys\n- https://docs.hookbridge.io/api/operations/listapikeys\ndescription: Authentication schemes for Hookbridge as documented.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: API keys authenticate requests to the HookBridge API.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key via the HookBridge console or API and copy the key; use it as a Bearer token in the Authorization header.\nnote: Hookbridge does not document any OAuth2, apiKey in query/body, or other authentication mechanisms.\ndocs: https://docs.hookbridge.io/guides/product/api-keys/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hookbridge/refs/heads/main/authentication/hookbridge-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Webhooks
- SaaS
- API
- Integration
---
