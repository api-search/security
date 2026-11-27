---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nextbid-us-account-api-openapi.yml
  format: yaml
  label: NextBid Account API
  slug: nextbid-us-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nextbid-us/openapi/nextbid-us-account-api-openapi.yml
- filename: nextbid-us-health-api-openapi.yml
  format: yaml
  label: NextBid Health API
  slug: nextbid-us-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nextbid-us/openapi/nextbid-us-health-api-openapi.yml
- filename: nextbid-us-opportunities-api-openapi.yml
  format: yaml
  label: NextBid Opportunities API
  slug: nextbid-us-opportunities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nextbid-us/openapi/nextbid-us-opportunities-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: NextBid Authentication
name_suffix: Authentication
oauth_flows: []
overview: NextBid secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NextBid
provider_slug: nextbid-us
scheme_count: 2
schemes:
- in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/nextbid-us-openapi.json
  type: apiKey
- name: BearerKey
  scheme: bearer
  sources:
  - openapi/nextbid-us-openapi.json
  type: http
slug: nextbid-us-authentication
source_filename: nextbid-us-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nextbid-us-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/nextbid-us-openapi.json\n- name: BearerKey\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/nextbid-us-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nextbid-us/authentication/nextbid-us-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Government Bids
- Small Business
- Procurement
- Artificial Intelligence
- Set‑asides
---
