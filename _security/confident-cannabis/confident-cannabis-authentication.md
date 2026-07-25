---
api_key_in:
- header
api_specs:
- filename: confident-cannabis-client-info-api-openapi.yml
  format: yaml
  label: Confident Cannabis Client Info API
  slug: confident-cannabis-client-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/openapi/confident-cannabis-client-info-api-openapi.yml
- filename: confident-cannabis-clients-api-openapi.yml
  format: yaml
  label: Confident Cannabis Clients API
  slug: confident-cannabis-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/openapi/confident-cannabis-clients-api-openapi.yml
- filename: confident-cannabis-lab-info-api-openapi.yml
  format: yaml
  label: Confident Cannabis Lab Info API
  slug: confident-cannabis-lab-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/openapi/confident-cannabis-lab-info-api-openapi.yml
- filename: confident-cannabis-labs-api-openapi.yml
  format: yaml
  label: Confident Cannabis Labs API
  slug: confident-cannabis-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/openapi/confident-cannabis-labs-api-openapi.yml
- filename: confident-cannabis-order-status-api-openapi.yml
  format: yaml
  label: Confident Cannabis Order Status API
  slug: confident-cannabis-order-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/openapi/confident-cannabis-order-status-api-openapi.yml
- filename: confident-cannabis-orders-api-openapi.yml
  format: yaml
  label: Confident Cannabis Orders API
  slug: confident-cannabis-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/openapi/confident-cannabis-orders-api-openapi.yml
- filename: confident-cannabis-reference-data-api-openapi.yml
  format: yaml
  label: Confident Cannabis Reference Data API
  slug: confident-cannabis-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/openapi/confident-cannabis-reference-data-api-openapi.yml
- filename: confident-cannabis-sample-files-api-openapi.yml
  format: yaml
  label: Confident Cannabis Sample Files API
  slug: confident-cannabis-sample-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/openapi/confident-cannabis-sample-files-api-openapi.yml
- filename: confident-cannabis-samples-api-openapi.yml
  format: yaml
  label: Confident Cannabis Samples API
  slug: confident-cannabis-samples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/openapi/confident-cannabis-samples-api-openapi.yml
- filename: confident-cannabis-test-results-api-openapi.yml
  format: yaml
  label: Confident Cannabis Test Results API
  slug: confident-cannabis-test-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/openapi/confident-cannabis-test-results-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Confident Cannabis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Confident Cannabis secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Confident Cannabis
provider_slug: confident-cannabis
scheme_count: 3
schemes:
- description: API key for authentication. Required for all requests.
  in: header
  name: ApiKeyAuth
  parameter: X-ConfidentCannabis-APIKey
  sources:
  - openapi/confident-cannabis-client-openapi.json
  - openapi/confident-cannabis-common-openapi.json
  - openapi/confident-cannabis-lab-openapi.json
  type: apiKey
- description: HMAC SHA256 signature (required if signing enabled)
  in: header
  name: SignatureAuth
  parameter: X-ConfidentCannabis-Signature
  sources:
  - openapi/confident-cannabis-lab-openapi.json
  type: apiKey
- description: Unix timestamp (required if signing enabled, must be within 30 seconds)
  in: header
  name: TimestampAuth
  parameter: X-ConfidentCannabis-Timestamp
  sources:
  - openapi/confident-cannabis-lab-openapi.json
  type: apiKey
slug: confident-cannabis-authentication
source_filename: confident-cannabis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/confident-cannabis-client-openapi.json, openapi/confident-cannabis-common-openapi.json,\n  openapi/confident-cannabis-lab-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-ConfidentCannabis-APIKey\n  description: API key for authentication. Required for all requests.\n  sources:\n  - openapi/confident-cannabis-client-openapi.json\n  - openapi/confident-cannabis-common-openapi.json\n  - openapi/confident-cannabis-lab-openapi.json\n- name: SignatureAuth\n  type: apiKey\n  in: header\n  parameter: X-ConfidentCannabis-Signature\n  description: HMAC SHA256 signature (required if signing enabled)\n  sources:\n  - openapi/confident-cannabis-lab-openapi.json\n- name: TimestampAuth\n  type: apiKey\n  in: header\n  parameter: X-ConfidentCannabis-Timestamp\n  description: Unix timestamp (required if signing enabled, must be within\
  \ 30 seconds)\n  sources:\n  - openapi/confident-cannabis-lab-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/authentication/confident-cannabis-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Cannabis
- Laboratory
- LIMS
- Testing
- Compliance
- Certificate of Analysis
- Life Sciences
---
