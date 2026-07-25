---
api_key_in:
- header
- query
api_specs:
- filename: steadily-account-api-openapi.yml
  format: yaml
  label: Steadily Account API
  slug: steadily-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-account-api-openapi.yml
- filename: steadily-draft-quote-api-openapi.yml
  format: yaml
  label: Steadily Draft Quote API
  slug: steadily-draft-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-draft-quote-api-openapi.yml
- filename: steadily-lead-referrals-api-openapi.yml
  format: yaml
  label: Steadily Lead Referrals API
  slug: steadily-lead-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-lead-referrals-api-openapi.yml
- filename: steadily-lender-api-openapi.yml
  format: yaml
  label: Steadily Lender API
  slug: steadily-lender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-lender-api-openapi.yml
- filename: steadily-policy-api-openapi.yml
  format: yaml
  label: Steadily Policy API
  slug: steadily-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-policy-api-openapi.yml
- filename: steadily-quote-estimates-api-openapi.yml
  format: yaml
  label: Steadily Quote Estimates API
  slug: steadily-quote-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-quote-estimates-api-openapi.yml
- filename: steadily-quote-offer-api-openapi.yml
  format: yaml
  label: Steadily Quote Offer API
  slug: steadily-quote-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-quote-offer-api-openapi.yml
- filename: steadily-reporting-api-openapi.yml
  format: yaml
  label: Steadily Reporting API
  slug: steadily-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadily/refs/heads/main/openapi/steadily-reporting-api-openapi.yml
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
