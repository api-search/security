---
api_key_in:
- header
api_specs:
- filename: trabex-aes-filing-api-openapi.yml
  format: yaml
  label: Trabex AES Filing API
  slug: trabex-aes-filing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trabex/refs/heads/main/openapi/trabex-aes-filing-api-openapi.yml
- filename: trabex-companies-api-openapi.yml
  format: yaml
  label: Trabex Companies API
  slug: trabex-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trabex/refs/heads/main/openapi/trabex-companies-api-openapi.yml
- filename: trabex-documents-api-openapi.yml
  format: yaml
  label: Trabex Documents API
  slug: trabex-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trabex/refs/heads/main/openapi/trabex-documents-api-openapi.yml
- filename: trabex-screening-api-openapi.yml
  format: yaml
  label: Trabex Screening API
  slug: trabex-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trabex/refs/heads/main/openapi/trabex-screening-api-openapi.yml
- filename: trabex-shipments-api-openapi.yml
  format: yaml
  label: Trabex Shipments API
  slug: trabex-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trabex/refs/heads/main/openapi/trabex-shipments-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trabex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trabex secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trabex
provider_slug: trabex
scheme_count: 1
schemes:
- description: Trabex API key for authenticating requests. Obtain your API key from the Trabex customer portal at support.trabex.io.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/trabex-trade-compliance-openapi.yml
  type: apiKey
slug: trabex-authentication
source_filename: trabex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trabex-trade-compliance-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Trabex API key for authenticating requests. Obtain your API key from the Trabex\n    customer portal at support.trabex.io.\n  sources:\n  - openapi/trabex-trade-compliance-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trabex/refs/heads/main/authentication/trabex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compliance
- Export Control
- Logistics
- Restricted Party Screening
- Shipment Management
- Trade Compliance
---
