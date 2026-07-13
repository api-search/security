---
api_key_in: []
api_specs:
- filename: old-dominion-freight-line-bill-of-lading-api-openapi.yml
  format: yaml
  label: ODFL Bill of Lading API
  slug: bill-of-lading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/old-dominion-freight-line/refs/heads/main/openapi/old-dominion-freight-line-bill-of-lading-api-openapi.yml
- filename: old-dominion-freight-line-pickup-api-openapi.yml
  format: yaml
  label: ODFL Pickup API
  slug: pickup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/old-dominion-freight-line/refs/heads/main/openapi/old-dominion-freight-line-pickup-api-openapi.yml
- filename: old-dominion-freight-line-tracking-api-openapi.yml
  format: yaml
  label: ODFL Tracking API
  slug: tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/old-dominion-freight-line/refs/heads/main/openapi/old-dominion-freight-line-tracking-api-openapi.yml
- filename: old-dominion-freight-line-document-api-openapi.yml
  format: yaml
  label: ODFL Document API
  slug: document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/old-dominion-freight-line/refs/heads/main/openapi/old-dominion-freight-line-document-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Old Dominion Freight Line Authentication
name_suffix: Authentication
oauth_flows: []
overview: Old Dominion Freight Line secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Old Dominion Freight Line
provider_slug: old-dominion-freight-line
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/old-dominion-freight-line-bill-of-lading-api-openapi.yml
  - openapi/old-dominion-freight-line-document-api-openapi.yml
  - openapi/old-dominion-freight-line-pickup-api-openapi.yml
  - openapi/old-dominion-freight-line-tracking-api-openapi.yml
  type: http
slug: old-dominion-freight-line-authentication
source_filename: old-dominion-freight-line-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/old-dominion-freight-line-bill-of-lading-api-openapi.yml, openapi/old-dominion-freight-line-document-api-openapi.yml,\n  openapi/old-dominion-freight-line-pickup-api-openapi.yml, openapi/old-dominion-freight-line-tracking-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/old-dominion-freight-line-bill-of-lading-api-openapi.yml\n  - openapi/old-dominion-freight-line-document-api-openapi.yml\n  - openapi/old-dominion-freight-line-pickup-api-openapi.yml\n  - openapi/old-dominion-freight-line-tracking-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/old-dominion-freight-line/refs/heads/main/authentication/old-dominion-freight-line-authentication.yml
summary_line: http · 1 scheme
tags:
- Freight
- Less-Than-Truckload
- Logistics
- Shipping
- Transportation
- Fortune 1000
---
