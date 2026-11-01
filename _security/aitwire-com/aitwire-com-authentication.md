---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: aitwire-com-api-keys-api-openapi.yml
  format: yaml
  label: aitwire-com API Keys API
  slug: aitwire-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-api-keys-api-openapi.yml
- filename: aitwire-com-attribution-api-openapi.yml
  format: yaml
  label: aitwire-com Attribution API
  slug: aitwire-com-attribution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-attribution-api-openapi.yml
- filename: aitwire-com-authority-api-openapi.yml
  format: yaml
  label: aitwire-com Authority API
  slug: aitwire-com-authority-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-authority-api-openapi.yml
- filename: aitwire-com-billing-api-openapi.yml
  format: yaml
  label: aitwire-com Billing API
  slug: aitwire-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-billing-api-openapi.yml
- filename: aitwire-com-drift-api-openapi.yml
  format: yaml
  label: aitwire-com Drift API
  slug: aitwire-com-drift-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-drift-api-openapi.yml
- filename: aitwire-com-entities-api-openapi.yml
  format: yaml
  label: aitwire-com Entities API
  slug: aitwire-com-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-entities-api-openapi.yml
- filename: aitwire-com-scans-api-openapi.yml
  format: yaml
  label: aitwire-com Scans API
  slug: aitwire-com-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-scans-api-openapi.yml
- filename: aitwire-com-webhooks-api-openapi.yml
  format: yaml
  label: aitwire-com Webhooks API
  slug: aitwire-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Aitwire Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: aitwire-com secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: aitwire-com
provider_slug: aitwire-com
scheme_count: 2
schemes:
- description: Bearer atwk_...
  name: ApiKeyBearer
  scheme: bearer
  sources:
  - openapi/aitwire-com-openapi.json
  type: http
- description: 'X-API-Key: atwk_...'
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/aitwire-com-openapi.json
  type: apiKey
slug: aitwire-com-authentication
source_filename: aitwire-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/aitwire-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyBearer\n  type: http\n  scheme: bearer\n  description: Bearer atwk_...\n  sources:\n  - openapi/aitwire-com-openapi.json\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'X-API-Key: atwk_...'\n  sources:\n  - openapi/aitwire-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/aitwire-com/authentication/aitwire-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- IoT
- Connectivity
- API
- Industrial
---
