---
api_key_in: []
api_specs:
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Screening API
  slug: sanctions-io-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Batch Screening API
  slug: sanctions-io-batch-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Adverse Media API
  slug: sanctions-io-adverse-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Data Sources API
  slug: sanctions-io-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Monitoring API
  slug: sanctions-io-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Account Management API
  slug: sanctions-io-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sanctions Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: sanctions.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: sanctions.io
provider_slug: sanctions-io
scheme_count: 1
schemes:
- description: 'API token from the sanctions.io user portal, passed as "Authorization: Bearer {token}". The token may also be sent as a URL parameter, but the Authorization header is recommended.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sanctions-io-openapi.yml
  type: http
slug: sanctions-io-authentication
source_filename: sanctions-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sanctions-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API token from the sanctions.io user portal, passed as \"Authorization: Bearer\n    {token}\". The token may also be sent as a URL parameter, but the Authorization header is\n    recommended.'\n  sources:\n  - openapi/sanctions-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/authentication/sanctions-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Anti-Money Laundering
- AML
- Sanctions Screening
- Compliance
- PEP Screening
- Watchlists
- KYC
- RegTech
---
