---
api_key_in:
- header
- query
api_specs:
- filename: amagi-add-user-api-openapi.yml
  format: yaml
  label: Amagi Add User API
  slug: amagi-add-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-add-user-api-openapi.yml
- filename: amagi-cancel-api-openapi.yml
  format: yaml
  label: Amagi Cancel API
  slug: amagi-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-cancel-api-openapi.yml
- filename: amagi-create-customer-api-openapi.yml
  format: yaml
  label: Amagi Create Customer API
  slug: amagi-create-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-create-customer-api-openapi.yml
- filename: amagi-delete-customer-api-openapi.yml
  format: yaml
  label: Amagi Delete Customer API
  slug: amagi-delete-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-delete-customer-api-openapi.yml
- filename: amagi-destroy-api-openapi.yml
  format: yaml
  label: Amagi Destroy API
  slug: amagi-destroy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-destroy-api-openapi.yml
- filename: amagi-disable-user-api-openapi.yml
  format: yaml
  label: Amagi Disable User API
  slug: amagi-disable-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-disable-user-api-openapi.yml
- filename: amagi-enable-user-api-openapi.yml
  format: yaml
  label: Amagi Enable User API
  slug: amagi-enable-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-enable-user-api-openapi.yml
- filename: amagi-get-info-api-openapi.yml
  format: yaml
  label: Amagi Get Info API
  slug: amagi-get-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-get-info-api-openapi.yml
- filename: amagi-get-key-api-openapi.yml
  format: yaml
  label: Amagi Get Key API
  slug: amagi-get-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-get-key-api-openapi.yml
- filename: amagi-get-metrics-api-openapi.yml
  format: yaml
  label: Amagi Get Metrics API
  slug: amagi-get-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-get-metrics-api-openapi.yml
- filename: amagi-head-key-api-openapi.yml
  format: yaml
  label: Amagi Head Key API
  slug: amagi-head-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-head-key-api-openapi.yml
- filename: amagi-list-api-openapi.yml
  format: yaml
  label: Amagi List API
  slug: amagi-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-list-api-openapi.yml
- filename: amagi-list-keys-api-openapi.yml
  format: yaml
  label: Amagi List Keys API
  slug: amagi-list-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-list-keys-api-openapi.yml
- filename: amagi-list-versions-api-openapi.yml
  format: yaml
  label: Amagi List Versions API
  slug: amagi-list-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-list-versions-api-openapi.yml
- filename: amagi-logs-api-openapi.yml
  format: yaml
  label: Amagi Logs API
  slug: amagi-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-logs-api-openapi.yml
- filename: amagi-regenerate-token-api-openapi.yml
  format: yaml
  label: Amagi Regenerate Token API
  slug: amagi-regenerate-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-regenerate-token-api-openapi.yml
- filename: amagi-retry-api-openapi.yml
  format: yaml
  label: Amagi Retry API
  slug: amagi-retry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-retry-api-openapi.yml
- filename: amagi-set-key-api-openapi.yml
  format: yaml
  label: Amagi Set Key API
  slug: amagi-set-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-set-key-api-openapi.yml
- filename: amagi-status-api-openapi.yml
  format: yaml
  label: Amagi Status API
  slug: amagi-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-status-api-openapi.yml
- filename: amagi-submit-api-openapi.yml
  format: yaml
  label: Amagi Submit API
  slug: amagi-submit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-submit-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amagi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amagi secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Amagi
provider_slug: amagi
scheme_count: 3
schemes:
- in: header
  name: access-key
  parameter: access_key
  sources:
  - openapi/amagi-callisto-openapi.yml
  type: apiKey
- in: header
  name: secret-key
  parameter: secret_key
  sources:
  - openapi/amagi-callisto-openapi.yml
  type: apiKey
- in: query
  name: TokenAuth
  parameter: token
  sources:
  - openapi/amagi-mapsor-openapi.yml
  type: apiKey
slug: amagi-authentication
source_filename: amagi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/amagi-callisto-openapi.yml, openapi/amagi-mapsor-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: access-key\n  type: apiKey\n  in: header\n  parameter: access_key\n  sources:\n  - openapi/amagi-callisto-openapi.yml\n- name: secret-key\n  type: apiKey\n  in: header\n  parameter: secret_key\n  sources:\n  - openapi/amagi-callisto-openapi.yml\n- name: TokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/amagi-mapsor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/authentication/amagi-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Media
- Broadcast
- Streaming
- Video
- CTV
- FAST
- Advertising
- Cloud
- Playout
---
