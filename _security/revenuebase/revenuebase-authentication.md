---
api_key_in:
- header
api_specs:
- filename: revenuebase-account-api-openapi.yml
  format: yaml
  label: RevenueBase Account API
  slug: revenuebase-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuebase/refs/heads/main/openapi/revenuebase-account-api-openapi.yml
- filename: revenuebase-email-api-openapi.yml
  format: yaml
  label: RevenueBase Email API
  slug: revenuebase-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuebase/refs/heads/main/openapi/revenuebase-email-api-openapi.yml
- filename: revenuebase-jobs-api-openapi.yml
  format: yaml
  label: RevenueBase Jobs API
  slug: revenuebase-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuebase/refs/heads/main/openapi/revenuebase-jobs-api-openapi.yml
- filename: revenuebase-organization-api-openapi.yml
  format: yaml
  label: RevenueBase Organization API
  slug: revenuebase-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuebase/refs/heads/main/openapi/revenuebase-organization-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Revenuebase Authentication
name_suffix: Authentication
oauth_flows: []
overview: RevenueBase secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RevenueBase
provider_slug: revenuebase
scheme_count: 1
schemes:
- dashboard: https://app.revenuebase.ai
  in: header
  name: APIKeyHeader
  parameter: x-key
  rotation_operation: rotate_api_key_v2_account_api_keys_rotate_post
  sources:
  - openapi/revenuebase-openapi.json
  - https://docs.revenuebase.ai/api-reference/authentication
  type: apiKey
slug: revenuebase-authentication
source_filename: revenuebase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/revenuebase-openapi.json\ndocs: https://docs.revenuebase.ai/api-reference/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    RevenueBase uses API key authentication exclusively. The key is passed in\n    the `x-key` request header (not `Authorization`, not `x-api-key`). Keys are\n    generated in the dashboard at https://app.revenuebase.ai under the Developers\n    section (Production API Key). No documented key prefix. Keys can be rotated\n    programmatically via POST /v2/account/api-keys/rotate, which immediately\n    invalidates the previous key.\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-key\n  dashboard: https://app.revenuebase.ai\n  rotation_operation: rotate_api_key_v2_account_api_keys_rotate_post\n  sources:\n  - openapi/revenuebase-openapi.json\n  - https://docs.revenuebase.ai/api-reference/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revenuebase/refs/heads/main/authentication/revenuebase-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- B2B Data
- Data Enrichment
- Email Verification
- Contact Data
- Company Data
- Lead Intelligence
- Sales Intelligence
---
