---
api_key_in: []
api_specs:
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Causes API
  slug: benevity-causes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Giving API
  slug: benevity-giving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Receipts API
  slug: benevity-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Spark Giving Opportunities API
  slug: benevity-spark-giving-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Spark Volunteer Opportunities API
  slug: benevity-spark-volunteer-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Benevity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Benevity secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Benevity
provider_slug: benevity
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/benevity-openapi.yml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/benevity-openapi.yml
  type: http
slug: benevity-authentication
source_filename: benevity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/benevity-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/benevity-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/benevity-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/authentication/benevity-authentication.yml
summary_line: http · 2 schemes
tags:
- Corporate Social Responsibility
- Workplace Giving
- Donations
- Volunteering
- Nonprofits
- Matching Gifts
- CSR
- ESG
---
