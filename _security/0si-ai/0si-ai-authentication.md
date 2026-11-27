---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 0si-ai-companies-api-openapi.yml
  format: yaml
  label: 공시.ai Companies API
  slug: 0si-ai-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-companies-api-openapi.yml
- filename: 0si-ai-disclosures-api-openapi.yml
  format: yaml
  label: 공시.ai Disclosures API
  slug: 0si-ai-disclosures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-disclosures-api-openapi.yml
- filename: 0si-ai-sec-api-openapi.yml
  format: yaml
  label: 공시.ai Sec API
  slug: 0si-ai-sec-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-sec-api-openapi.yml
- filename: 0si-ai-status-api-openapi.yml
  format: yaml
  label: 공시.ai Status API
  slug: 0si-ai-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-status-api-openapi.yml
- filename: 0si-ai-stream-api-openapi.yml
  format: yaml
  label: 공시.ai Stream API
  slug: 0si-ai-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-stream-api-openapi.yml
- filename: 0si-ai-usage-api-openapi.yml
  format: yaml
  label: 공시.ai Usage API
  slug: 0si-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-usage-api-openapi.yml
- filename: 0si-ai-webhooks-api-openapi.yml
  format: yaml
  label: 공시.ai Webhooks API
  slug: 0si-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: 공시.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: 공시.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: 공시.ai
provider_slug: 0si-ai
scheme_count: 2
schemes:
- description: API key header for authentication.
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: Bearer token authentication using API key.
  scheme: bearer
  type: http
slug: 0si-ai-authentication
source_filename: 0si-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://0si.ai/developers\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: \"API key header for authentication.\"\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"Bearer token authentication using API key.\"\n"
source_yaml_url: https://artifacts.apis.io/0si-ai/authentication/0si-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Finance
- Filings
- South Korea
- USA
---
