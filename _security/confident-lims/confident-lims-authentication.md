---
api_key_in:
- header
api_specs:
- filename: confident-lims-labs-openapi.json
  format: json
  label: Confident Cannabis API - Lab Endpoints
  slug: confident-cannabis-api-lab-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-labs-openapi.json
- filename: confident-lims-clients-openapi.json
  format: json
  label: Confident Cannabis API - Client Endpoints
  slug: confident-cannabis-api-client-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-clients-openapi.json
- filename: confident-lims-common-openapi.json
  format: json
  label: Confident Cannabis API - Common Reference Data
  slug: confident-cannabis-api-common-reference-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-common-openapi.json
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
