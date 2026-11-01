---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: layercall-com-ai-agents-api-openapi.yml
  format: yaml
  label: layercall-com AI agents API
  slug: layercall-com-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-ai-agents-api-openapi.yml
- filename: layercall-com-batch-api-openapi.yml
  format: yaml
  label: layercall-com Batch API
  slug: layercall-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-batch-api-openapi.yml
- filename: layercall-com-device-api-openapi.yml
  format: yaml
  label: layercall-com Device API
  slug: layercall-com-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-device-api-openapi.yml
- filename: layercall-com-reputation-api-openapi.yml
  format: yaml
  label: layercall-com Reputation API
  slug: layercall-com-reputation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-reputation-api-openapi.yml
- filename: layercall-com-rules-api-openapi.yml
  format: yaml
  label: layercall-com Rules API
  slug: layercall-com-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-rules-api-openapi.yml
- filename: layercall-com-scoring-api-openapi.yml
  format: yaml
  label: layercall-com Scoring API
  slug: layercall-com-scoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-scoring-api-openapi.yml
- filename: layercall-com-unified-api-openapi.yml
  format: yaml
  label: layercall-com Unified API
  slug: layercall-com-unified-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-unified-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Layercall Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: layercall-com secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: layercall-com
provider_slug: layercall-com
scheme_count: 2
schemes:
- description: Your API key from https://www.layercall.com/get-key
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/layercall-com-openapi.json
  type: apiKey
- description: 'Same key, sent as `Authorization: Bearer <key>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/layercall-com-openapi.json
  type: http
slug: layercall-com-authentication
source_filename: layercall-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/layercall-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Your API key from https://www.layercall.com/get-key\n  sources:\n  - openapi/layercall-com-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Same key, sent as `Authorization: Bearer <key>`.'\n  sources:\n  - openapi/layercall-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/layercall-com/authentication/layercall-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- FraudDetection
- TrustIntelligence
- API
- Security
---
