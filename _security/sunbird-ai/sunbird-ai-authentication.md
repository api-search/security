---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sunbird-ai-api-openapi.json
  format: json
  label: Sunbird AI API API
  slug: sunbird-ai-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sunbird-ai/openapi/_original/sunbird-ai-api-openapi.json
auth_types: []
description: Authentication schemes for Sunbird AI API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sunbird AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sunbird AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Sunbird AI
provider_slug: sunbird-ai
scheme_count: 1
schemes:
- evidence: The Sunbird AI API uses **Bearer Token** authentication. You must include a valid access token in the `Authorization` header of your HTTP requests.
  header: Authorization
  how_to_obtain: Obtain an access token by POSTing form‑encoded credentials (username and password) to the `/auth/token` endpoint.
  location: header
  name: Bearer Token
  token_url: https://api.sunbird.ai/auth/token
  type: http-bearer
slug: sunbird-ai-authentication
source_filename: sunbird-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.sunbird.ai/authentication.md
source_yaml: "generated: '2026-11-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.sunbird.ai/authentication.md\nsources:\n- https://docs.sunbird.ai/authentication.md\n- https://docs.sunbird.ai/api-reference/authentication/register.md\n- https://docs.sunbird.ai/api-reference/authentication/verify-email.md\n- https://docs.sunbird.ai/api-reference/authentication/resend-verification.md\ndescription: Authentication schemes for Sunbird AI API\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: The Sunbird AI API uses **Bearer Token** authentication. You must include a valid access token in the `Authorization` header of your\n    HTTP requests.\n  location: header\n  header: Authorization\n  token_url: https://api.sunbird.ai/auth/token\n  how_to_obtain: Obtain an access token by POSTing form‑encoded credentials (username and password) to the `/auth/token` endpoint.\nnote: No OAuth2, apiKey, or other authentication types are documented.\ndocs:\
  \ https://docs.sunbird.ai/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/sunbird-ai/authentication/sunbird-ai-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Non-profit
- Social Impact
- Uganda
- Machine Learning
---
