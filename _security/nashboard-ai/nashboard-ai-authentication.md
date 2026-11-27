---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nashboard-ai-flywheel-api-openapi.yml
  format: yaml
  label: Nashboard Flywheel API
  slug: nashboard-ai-flywheel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nashboard-ai/openapi/nashboard-ai-flywheel-api-openapi.yml
- filename: nashboard-ai-key-management-api-openapi.yml
  format: yaml
  label: Nashboard Key Management API
  slug: nashboard-ai-key-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nashboard-ai/openapi/nashboard-ai-key-management-api-openapi.yml
- filename: nashboard-ai-merchant-enrichment-api-openapi.yml
  format: yaml
  label: Nashboard Merchant Enrichment API
  slug: nashboard-ai-merchant-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nashboard-ai/openapi/nashboard-ai-merchant-enrichment-api-openapi.yml
- filename: nashboard-ai-public-api-openapi.yml
  format: yaml
  label: Nashboard Public API
  slug: nashboard-ai-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nashboard-ai/openapi/nashboard-ai-public-api-openapi.yml
- filename: nashboard-ai-receipt-ocr-api-openapi.yml
  format: yaml
  label: Nashboard Receipt OCR API
  slug: nashboard-ai-receipt-ocr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nashboard-ai/openapi/nashboard-ai-receipt-ocr-api-openapi.yml
- filename: nashboard-ai-self-serve-api-openapi.yml
  format: yaml
  label: Nashboard Self Serve API
  slug: nashboard-ai-self-serve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nashboard-ai/openapi/nashboard-ai-self-serve-api-openapi.yml
- filename: nashboard-ai-usage-sla-api-openapi.yml
  format: yaml
  label: Nashboard Usage & SLA API
  slug: nashboard-ai-usage-sla-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nashboard-ai/openapi/nashboard-ai-usage-sla-api-openapi.yml
- filename: nashboard-ai-webhooks-api-openapi.yml
  format: yaml
  label: Nashboard Webhooks API
  slug: nashboard-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nashboard-ai/openapi/nashboard-ai-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Nashboard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nashboard secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nashboard
provider_slug: nashboard-ai
scheme_count: 2
schemes:
- description: 'API key as a Bearer token: `Authorization: Bearer nsh_live_...`'
  name: apiKeyBearer
  scheme: bearer
  sources:
  - openapi/nashboard-ai-openapi.json
  type: http
- description: 'API key as a custom header: `X-API-Key: nsh_live_...`'
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/nashboard-ai-openapi.json
  type: apiKey
slug: nashboard-ai-authentication
source_filename: nashboard-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nashboard-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  description: 'API key as a Bearer token: `Authorization: Bearer nsh_live_...`'\n  sources:\n  - openapi/nashboard-ai-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'API key as a custom header: `X-API-Key: nsh_live_...`'\n  sources:\n  - openapi/nashboard-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nashboard-ai/authentication/nashboard-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Finance
- Personal Finance
- iOS
- Artificial Intelligence
- Privacy
---
