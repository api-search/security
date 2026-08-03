---
api_key_in:
- header
api_specs:
- filename: anomalo-public-api-openapi.yml
  format: yaml
  label: Anomalo Public API
  slug: anomalo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-public-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Anomalo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anomalo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Anomalo
provider_slug: anomalo
scheme_count: 2
schemes:
- description: Anomalo API secret token. The first-party client sends it as `X-Anomalo-Token` by default (`legacy_auth=True`), read from the `ANOMALO_API_SECRET_TOKEN` environment variable.
  in: header
  name: AnomaloToken
  parameter: X-Anomalo-Token
  sources:
  - openapi/anomalo-public-api-openapi.yml
  type: apiKey
- description: 'Anomalo API secret token sent as `Authorization: Bearer <token>`. Selected in the first-party client with `legacy_auth=False`.'
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/anomalo-public-api-openapi.yml
  type: http
slug: anomalo-authentication
source_filename: anomalo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: derived\nsource: openapi/anomalo-public-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: AnomaloToken\n  type: apiKey\n  in: header\n  parameter: X-Anomalo-Token\n  description: Anomalo API secret token. The first-party client sends it as `X-Anomalo-Token`\n    by default (`legacy_auth=True`), read from the `ANOMALO_API_SECRET_TOKEN` environment variable.\n  sources:\n  - openapi/anomalo-public-api-openapi.yml\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: 'Anomalo API secret token sent as `Authorization: Bearer <token>`. Selected in\n    the first-party client with `legacy_auth=False`.'\n  sources:\n  - openapi/anomalo-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/authentication/anomalo-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- data-quality
- data-observability
- data-monitoring
- anomaly-detection
- data-governance
- data-lineage
- data-profiling
- data-validation
- data-engineering
- machine-learning
- snowflake
- databricks
- bigquery
- enterprise-data
- mcp
- agent-native
---
