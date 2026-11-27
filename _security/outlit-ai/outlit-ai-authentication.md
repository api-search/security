---
anonymous_access: false
api_key_in: []
api_specs:
- filename: outlit-ai-feedback-api-openapi.yml
  format: yaml
  label: Outlit Feedback API
  slug: outlit-ai-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outlit-ai/openapi/outlit-ai-feedback-api-openapi.yml
- filename: outlit-ai-i-api-openapi.yml
  format: yaml
  label: Outlit I API
  slug: outlit-ai-i-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outlit-ai/openapi/outlit-ai-i-api-openapi.yml
- filename: outlit-ai-tools-api-openapi.yml
  format: yaml
  label: Outlit Tools API
  slug: outlit-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outlit-ai/openapi/outlit-ai-tools-api-openapi.yml
- filename: outlit-ai-validate-api-key-api-openapi.yml
  format: yaml
  label: Outlit Validate Api Key API
  slug: outlit-ai-validate-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outlit-ai/openapi/outlit-ai-validate-api-key-api-openapi.yml
auth_types: []
description: Outlit API uses a bearer token passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Outlit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Outlit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Outlit
provider_slug: outlit-ai
scheme_count: 1
schemes:
- evidence: Pass an Outlit API key in the `Authorization` header as `Bearer ok_...`.
  header: Authorization
  how_to_obtain: Create an API key in the Outlit workspace Settings → API keys page; the key will have the prefix `ok_`.
  location: header
  name: bearerAuth
  type: http-bearer
slug: outlit-ai-authentication
source_filename: outlit-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.outlit.ai/api-reference/validation.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.outlit.ai/api-reference/validation.md\nsources:\n- https://docs.outlit.ai/api-reference/validation.md\n- https://docs.outlit.ai/getting-started/overview.md\n- https://docs.outlit.ai/getting-started/connect-data.md\n- https://docs.outlit.ai/getting-started/first-attention-item.md\ndescription: Outlit API uses a bearer token passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: bearerAuth\n  evidence: Pass an Outlit API key in the `Authorization` header as `Bearer ok_...`.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the Outlit workspace Settings → API keys page; the key will have the prefix `ok_`.\ndocs: https://docs.outlit.ai/api-reference/validation.md\n"
source_yaml_url: https://artifacts.apis.io/outlit-ai/authentication/outlit-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Customer Success
- Software-as-a-Service
- Integration Platform
- Y Combinator
---
