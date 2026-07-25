---
api_key_in:
- header
api_specs:
- filename: parseflow-admin-api-openapi.yml
  format: yaml
  label: Parseflow Admin API
  slug: parseflow-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-admin-api-openapi.yml
- filename: parseflow-analyze-api-openapi.yml
  format: yaml
  label: Parseflow Analyze API
  slug: parseflow-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-analyze-api-openapi.yml
- filename: parseflow-batch-api-openapi.yml
  format: yaml
  label: Parseflow Batch API
  slug: parseflow-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-batch-api-openapi.yml
- filename: parseflow-billing-api-openapi.yml
  format: yaml
  label: Parseflow Billing API
  slug: parseflow-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-billing-api-openapi.yml
- filename: parseflow-health-api-openapi.yml
  format: yaml
  label: Parseflow Health API
  slug: parseflow-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-health-api-openapi.yml
- filename: parseflow-index-api-openapi.yml
  format: yaml
  label: Parseflow Index API
  slug: parseflow-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-index-api-openapi.yml
- filename: parseflow-jobs-api-openapi.yml
  format: yaml
  label: Parseflow Jobs API
  slug: parseflow-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-jobs-api-openapi.yml
- filename: parseflow-me-api-openapi.yml
  format: yaml
  label: Parseflow Me API
  slug: parseflow-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-me-api-openapi.yml
- filename: parseflow-pack-api-openapi.yml
  format: yaml
  label: Parseflow Pack API
  slug: parseflow-pack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-pack-api-openapi.yml
- filename: parseflow-process-api-openapi.yml
  format: yaml
  label: Parseflow Process API
  slug: parseflow-process-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-process-api-openapi.yml
- filename: parseflow-search-api-openapi.yml
  format: yaml
  label: Parseflow Search API
  slug: parseflow-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-search-api-openapi.yml
- filename: parseflow-stats-api-openapi.yml
  format: yaml
  label: Parseflow Stats API
  slug: parseflow-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-stats-api-openapi.yml
- filename: parseflow-usage-api-openapi.yml
  format: yaml
  label: Parseflow Usage API
  slug: parseflow-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-usage-api-openapi.yml
- filename: parseflow-webhooks-api-openapi.yml
  format: yaml
  label: Parseflow Webhooks API
  slug: parseflow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/openapi/parseflow-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Parseflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parseflow secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parseflow
provider_slug: parseflow
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/parseflow-openapi.json
  type: apiKey
slug: parseflow-authentication
source_filename: parseflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parseflow-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/parseflow-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/authentication/parseflow-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Document Parsing
- PDF
- OCR
- Text Extraction
- Document AI
- Search
- BYOK
- Async Jobs
- Webhooks
- REST
---
