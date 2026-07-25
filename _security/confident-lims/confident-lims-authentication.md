---
api_key_in:
- header
api_specs:
- filename: confident-lims-client-info-api-openapi.yml
  format: yaml
  label: Confident LIMS Client Info API
  slug: confident-lims-client-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-client-info-api-openapi.yml
- filename: confident-lims-clients-api-openapi.yml
  format: yaml
  label: Confident LIMS Clients API
  slug: confident-lims-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-clients-api-openapi.yml
- filename: confident-lims-lab-info-api-openapi.yml
  format: yaml
  label: Confident LIMS Lab Info API
  slug: confident-lims-lab-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-lab-info-api-openapi.yml
- filename: confident-lims-labs-api-openapi.yml
  format: yaml
  label: Confident LIMS Labs API
  slug: confident-lims-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-labs-api-openapi.yml
- filename: confident-lims-order-status-api-openapi.yml
  format: yaml
  label: Confident LIMS Order Status API
  slug: confident-lims-order-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-order-status-api-openapi.yml
- filename: confident-lims-orders-api-openapi.yml
  format: yaml
  label: Confident LIMS Orders API
  slug: confident-lims-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-orders-api-openapi.yml
- filename: confident-lims-reference-data-api-openapi.yml
  format: yaml
  label: Confident LIMS Reference Data API
  slug: confident-lims-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-reference-data-api-openapi.yml
- filename: confident-lims-sample-files-api-openapi.yml
  format: yaml
  label: Confident LIMS Sample Files API
  slug: confident-lims-sample-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-sample-files-api-openapi.yml
- filename: confident-lims-samples-api-openapi.yml
  format: yaml
  label: Confident LIMS Samples API
  slug: confident-lims-samples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-samples-api-openapi.yml
- filename: confident-lims-test-results-api-openapi.yml
  format: yaml
  label: Confident LIMS Test Results API
  slug: confident-lims-test-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-test-results-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Confident Lims Authentication
name_suffix: Authentication
oauth_flows: []
overview: Confident LIMS secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Confident LIMS
provider_slug: confident-lims
scheme_count: 3
schemes:
- description: API key for authentication. Required for all requests.
  in: header
  name: ApiKeyAuth
  parameter: X-ConfidentCannabis-APIKey
  sources:
  - openapi/confident-lims-clients-openapi.json
  - openapi/confident-lims-common-openapi.json
  - openapi/confident-lims-labs-openapi.json
  type: apiKey
- description: HMAC SHA256 signature of the request. Required if signing is enabled for your API credentials.
  in: header
  name: SignatureAuth
  parameter: X-ConfidentCannabis-Signature
  sources:
  - openapi/confident-lims-clients-openapi.json
  - openapi/confident-lims-common-openapi.json
  - openapi/confident-lims-labs-openapi.json
  type: apiKey
- description: Unix timestamp of the request. Required if signing is enabled. Must be within 30 seconds of server time.
  in: header
  name: TimestampAuth
  parameter: X-ConfidentCannabis-Timestamp
  sources:
  - openapi/confident-lims-clients-openapi.json
  - openapi/confident-lims-common-openapi.json
  - openapi/confident-lims-labs-openapi.json
  type: apiKey
slug: confident-lims-authentication
source_filename: confident-lims-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/confident-lims-clients-openapi.json, openapi/confident-lims-common-openapi.json,\n  openapi/confident-lims-labs-openapi.json\ndocs: https://confidentlims.readme.io/reference/authentication\nmodel: API key + HMAC-SHA256 request signing. Three headers required on every request; the\n  timestamp must be within 30 seconds of server time (replay protection). API key + secret are\n  issued from account settings; the API is free for approved integration partners.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-ConfidentCannabis-APIKey\n  description: API key for authentication. Required for all requests.\n  sources:\n  - openapi/confident-lims-clients-openapi.json\n  - openapi/confident-lims-common-openapi.json\n  - openapi/confident-lims-labs-openapi.json\n- name: SignatureAuth\n  type: apiKey\n  in: header\n  parameter: X-ConfidentCannabis-Signature\n\
  \  description: HMAC SHA256 signature of the request. Required if signing is enabled for your\n    API credentials.\n  sources:\n  - openapi/confident-lims-clients-openapi.json\n  - openapi/confident-lims-common-openapi.json\n  - openapi/confident-lims-labs-openapi.json\n- name: TimestampAuth\n  type: apiKey\n  in: header\n  parameter: X-ConfidentCannabis-Timestamp\n  description: Unix timestamp of the request. Required if signing is enabled. Must be within\n    30 seconds of server time.\n  sources:\n  - openapi/confident-lims-clients-openapi.json\n  - openapi/confident-lims-common-openapi.json\n  - openapi/confident-lims-labs-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/authentication/confident-lims-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- LIMS
- Laboratory Information Management
- Analytical Testing
- Cannabis Testing
- Compliance
- Sample Management
- Lab Software
---
