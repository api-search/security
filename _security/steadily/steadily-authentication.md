---
api_key_in:
- header
- query
api_specs:
- filename: steadily-partner-openapi-original.json
  format: json
  label: Steadily Partner API
  slug: steadily-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-partner-openapi-original.json
- filename: steadily-estimate-api-openapi-original.json
  format: json
  label: Steadily Partner (Estimate) API
  slug: steadily-partner-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-estimate-api-openapi-original.json
- filename: steadily-rater-quotes-openapi-original.json
  format: json
  label: Steadily Rater Quotes API
  slug: steadily-rater-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-rater-quotes-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Steadily Authentication
name_suffix: Authentication
oauth_flows: []
overview: Steadily secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Steadily
provider_slug: steadily
scheme_count: 5
schemes:
- in: query
  name: APIKeyQuery
  parameter: X-Steadily-ApiKey
  sources:
  - openapi/steadily-estimate-api-openapi-original.json
  - openapi/steadily-partner-openapi-original.json
  - openapi/steadily-rater-quotes-openapi-original.json
  type: apiKey
- in: header
  name: APIKeyHeader
  parameter: X-Steadily-ApiKey
  sources:
  - openapi/steadily-estimate-api-openapi-original.json
  - openapi/steadily-partner-openapi-original.json
  - openapi/steadily-rater-quotes-openapi-original.json
  type: apiKey
- in: query
  name: SecretKeyQuery
  parameter: X-Steadily-SecretKey
  sources:
  - openapi/steadily-estimate-api-openapi-original.json
  - openapi/steadily-partner-openapi-original.json
  type: apiKey
- in: header
  name: SecretKeyHeader
  parameter: X-Steadily-SecretKey
  sources:
  - openapi/steadily-estimate-api-openapi-original.json
  - openapi/steadily-partner-openapi-original.json
  type: apiKey
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/steadily-partner-openapi-original.json
  - openapi/steadily-rater-quotes-openapi-original.json
  type: http
slug: steadily-authentication
source_filename: steadily-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/steadily-estimate-api-openapi-original.json, openapi/steadily-partner-openapi-original.json,\n  openapi/steadily-rater-quotes-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: APIKeyQuery\n  type: apiKey\n  in: query\n  parameter: X-Steadily-ApiKey\n  sources:\n  - openapi/steadily-estimate-api-openapi-original.json\n  - openapi/steadily-partner-openapi-original.json\n  - openapi/steadily-rater-quotes-openapi-original.json\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Steadily-ApiKey\n  sources:\n  - openapi/steadily-estimate-api-openapi-original.json\n  - openapi/steadily-partner-openapi-original.json\n  - openapi/steadily-rater-quotes-openapi-original.json\n- name: SecretKeyQuery\n  type: apiKey\n  in: query\n  parameter: X-Steadily-SecretKey\n  sources:\n  - openapi/steadily-estimate-api-openapi-original.json\n  - openapi/steadily-partner-openapi-original.json\n\
  - name: SecretKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Steadily-SecretKey\n  sources:\n  - openapi/steadily-estimate-api-openapi-original.json\n  - openapi/steadily-partner-openapi-original.json\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/steadily-partner-openapi-original.json\n  - openapi/steadily-rater-quotes-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/authentication/steadily-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Company
- Fintech
- Insurance
- Landlord Insurance
- Insurtech
- Real Estate
- Rental Property
- API
---
