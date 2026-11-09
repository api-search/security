---
anonymous_access: false
api_key_in: []
api_specs:
- filename: boxcompute-ai-openapi.yml
  format: yaml
  label: BoxCompute Customer Sandbox API
  slug: boxcompute-customer-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boxcompute-ai/openapi/boxcompute-ai-openapi.yml
auth_types: []
description: BoxCompute authenticates API requests using an API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Boxcompute Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: BoxCompute declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BoxCompute
provider_slug: boxcompute-ai
scheme_count: 1
schemes:
- evidence: 'Send the secret only in the HTTPS authorization header: Authorization: Bearer bc_live_REDACTED'
  header: Authorization
  how_to_obtain: Create an API key in the BoxCompute web app; the secret is shown once as a bc_live_... string.
  location: header
  name: Authorization
  type: apiKey
slug: boxcompute-ai-authentication
source_filename: boxcompute-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://boxcompute.ai/docs/api-keys/
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://boxcompute.ai/docs/api-keys/\nsources:\n- https://boxcompute.ai/docs/api-keys/\n- https://boxcompute.ai/docs/api-keys/index.md\n- https://boxcompute.ai/docs/quickstart/\n- https://boxcompute.ai/docs/quickstart/index.md\ndescription: BoxCompute authenticates API requests using an API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'Send the secret only in the HTTPS authorization header: Authorization: Bearer bc_live_REDACTED'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the BoxCompute web app; the secret is shown once as a bc_live_... string.\nnote: No OAuth2, HTTP Basic, JWT, HMAC, or mTLS schemes are documented.\ndocs: https://boxcompute.ai/docs/api-keys/\n"
source_yaml_url: https://artifacts.apis.io/boxcompute-ai/authentication/boxcompute-ai-authentication.yml
summary_line: 1 scheme
tags:
- AI Agents
- Pay-as-you-go
- Sandbox
---
