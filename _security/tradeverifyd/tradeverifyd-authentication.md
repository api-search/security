---
api_key_in:
- header
api_specs:
- filename: tradeverifyd-documents-api-openapi.yml
  format: yaml
  label: Tradeverifyd Documents API
  slug: tradeverifyd-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-documents-api-openapi.yml
- filename: tradeverifyd-entity-api-openapi.yml
  format: yaml
  label: Tradeverifyd Entity API
  slug: tradeverifyd-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-entity-api-openapi.yml
- filename: tradeverifyd-flags-api-openapi.yml
  format: yaml
  label: Tradeverifyd Flags API
  slug: tradeverifyd-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-flags-api-openapi.yml
- filename: tradeverifyd-organizations-api-openapi.yml
  format: yaml
  label: Tradeverifyd Organizations API
  slug: tradeverifyd-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-organizations-api-openapi.yml
- filename: tradeverifyd-relationships-api-openapi.yml
  format: yaml
  label: Tradeverifyd Relationships API
  slug: tradeverifyd-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-relationships-api-openapi.yml
- filename: tradeverifyd-reports-api-openapi.yml
  format: yaml
  label: Tradeverifyd Reports API
  slug: tradeverifyd-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-reports-api-openapi.yml
- filename: tradeverifyd-risk-events-api-openapi.yml
  format: yaml
  label: Tradeverifyd Risk Events API
  slug: tradeverifyd-risk-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-risk-events-api-openapi.yml
- filename: tradeverifyd-scitt-reference-apis-api-openapi.yml
  format: yaml
  label: Tradeverifyd SCITT Reference APIs API
  slug: tradeverifyd-scitt-reference-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-scitt-reference-apis-api-openapi.yml
- filename: tradeverifyd-shipments-api-openapi.yml
  format: yaml
  label: Tradeverifyd Shipments API
  slug: tradeverifyd-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-shipments-api-openapi.yml
- filename: tradeverifyd-system-api-openapi.yml
  format: yaml
  label: Tradeverifyd System API
  slug: tradeverifyd-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-system-api-openapi.yml
- filename: tradeverifyd-transparency-log-api-openapi.yml
  format: yaml
  label: Tradeverifyd Transparency Log API
  slug: tradeverifyd-transparency-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-transparency-log-api-openapi.yml
- filename: tradeverifyd-us-customs-api-openapi.yml
  format: yaml
  label: Tradeverifyd US Customs API
  slug: tradeverifyd-us-customs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-us-customs-api-openapi.yml
- filename: tradeverifyd-verifiable-credentials-api-openapi.yml
  format: yaml
  label: Tradeverifyd Verifiable Credentials API
  slug: tradeverifyd-verifiable-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/openapi/tradeverifyd-verifiable-credentials-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tradeverifyd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tradeverifyd secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tradeverifyd
provider_slug: tradeverifyd
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: ocp-apim-subscription-key
  sources:
  - openapi/tradeverifyd-openapi-original.json
  type: apiKey
slug: tradeverifyd-authentication
source_filename: tradeverifyd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/tradeverifyd-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: ocp-apim-subscription-key\n  sources:\n  - openapi/tradeverifyd-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradeverifyd/refs/heads/main/authentication/tradeverifyd-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Supply Chain
- Trade Compliance
- Risk Management
- Verifiable Credentials
- Customs
- Entity Resolution
- Logistics
---
