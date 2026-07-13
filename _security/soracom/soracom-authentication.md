---
api_key_in:
- header
api_specs:
- filename: soracom-sim-api-openapi.yml
  format: yaml
  label: Soracom SIM Management API
  slug: soracom-sim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-sim-api-openapi.yml
- filename: soracom-group-api-openapi.yml
  format: yaml
  label: Soracom Group Configuration API
  slug: soracom-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-group-api-openapi.yml
- filename: soracom-harvest-api-openapi.yml
  format: yaml
  label: Soracom Harvest API
  slug: soracom-harvest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-harvest-api-openapi.yml
- filename: soracom-inventory-api-openapi.yml
  format: yaml
  label: Soracom Inventory API
  slug: soracom-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-inventory-api-openapi.yml
- filename: soracom-napter-api-openapi.yml
  format: yaml
  label: Soracom Napter API
  slug: soracom-napter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-napter-api-openapi.yml
- filename: soracom-event-handler-api-openapi.yml
  format: yaml
  label: Soracom Event Handler API
  slug: soracom-event-handler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-event-handler-api-openapi.yml
- filename: soracom-vpg-api-openapi.yml
  format: yaml
  label: Soracom Virtual Private Gateway API
  slug: soracom-vpg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-vpg-api-openapi.yml
- filename: soracom-billing-api-openapi.yml
  format: yaml
  label: Soracom Billing API
  slug: soracom-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-billing-api-openapi.yml
- filename: soracom-stats-api-openapi.yml
  format: yaml
  label: Soracom Stats and Diagnostics API
  slug: soracom-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-stats-api-openapi.yml
- filename: soracom-auth-api-openapi.yml
  format: yaml
  label: Soracom Auth and Access Management API
  slug: soracom-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-auth-api-openapi.yml
- filename: soracom-analysis-query-api-openapi.yml
  format: yaml
  label: Soracom Analysis and Query API
  slug: soracom-analysis-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-analysis-query-api-openapi.yml
- filename: soracom-lagoon-api-openapi.yml
  format: yaml
  label: Soracom Lagoon API
  slug: soracom-lagoon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-lagoon-api-openapi.yml
- filename: soracom-lorawan-api-openapi.yml
  format: yaml
  label: Soracom Air for LoRaWAN API
  slug: soracom-lorawan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-lorawan-api-openapi.yml
- filename: soracom-sigfox-api-openapi.yml
  format: yaml
  label: Soracom Air for Sigfox API
  slug: soracom-sigfox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-sigfox-api-openapi.yml
- filename: soracom-soracam-api-openapi.yml
  format: yaml
  label: Soracom Cloud Camera Services API
  slug: soracom-soracam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-soracam-api-openapi.yml
- filename: soracom-batch-api-openapi.yml
  format: yaml
  label: Soracom Batch API
  slug: soracom-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-batch-api-openapi.yml
- filename: soracom-platform-api-openapi.yml
  format: yaml
  label: Soracom Platform API (Aggregate)
  slug: soracom-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-platform-api-openapi.yml
- filename: soracom-sandbox-api-openapi.yml
  format: yaml
  label: Soracom Sandbox API
  slug: soracom-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/openapi/soracom-sandbox-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Soracom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soracom secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Soracom
provider_slug: soracom
scheme_count: 2
schemes:
- description: 'API key for authentication. Obtain this from the Soracom User Console or via the Auth API.

    Required in combination with an API token for all authenticated requests.'
  in: header
  name: api_key
  parameter: X-Soracom-API-Key
  sources:
  - openapi/soracom-analysis-query-api-openapi.yml
  - openapi/soracom-auth-api-openapi.yml
  - openapi/soracom-batch-api-openapi.yml
  - openapi/soracom-billing-api-openapi.yml
  - openapi/soracom-event-handler-api-openapi.yml
  - openapi/soracom-group-api-openapi.yml
  - openapi/soracom-harvest-api-openapi.yml
  - openapi/soracom-inventory-api-openapi.yml
  - openapi/soracom-lagoon-api-openapi.yml
  - openapi/soracom-lorawan-api-openapi.yml
  - openapi/soracom-napter-api-openapi.yml
  - openapi/soracom-platform-api-openapi.yml
  - openapi/soracom-sigfox-api-openapi.yml
  - openapi/soracom-sim-api-openapi.yml
  - openapi/soracom-soracam-api-openapi.yml
  - openapi/soracom-stats-api-openapi.yml
  - openapi/soracom-vpg-api-openapi.yml
  type: apiKey
- description: 'API token for authentication. This token has an expiration time and must be refreshed periodically.

    Required in combination with an API key for all authenticated requests.'
  in: header
  name: api_token
  parameter: X-Soracom-Token
  sources:
  - openapi/soracom-analysis-query-api-openapi.yml
  - openapi/soracom-auth-api-openapi.yml
  - openapi/soracom-batch-api-openapi.yml
  - openapi/soracom-billing-api-openapi.yml
  - openapi/soracom-event-handler-api-openapi.yml
  - openapi/soracom-group-api-openapi.yml
  - openapi/soracom-harvest-api-openapi.yml
  - openapi/soracom-inventory-api-openapi.yml
  - openapi/soracom-lagoon-api-openapi.yml
  - openapi/soracom-lorawan-api-openapi.yml
  - openapi/soracom-napter-api-openapi.yml
  - openapi/soracom-platform-api-openapi.yml
  - openapi/soracom-sigfox-api-openapi.yml
  - openapi/soracom-sim-api-openapi.yml
  - openapi/soracom-soracam-api-openapi.yml
  - openapi/soracom-stats-api-openapi.yml
  - openapi/soracom-vpg-api-openapi.yml
  type: apiKey
slug: soracom-authentication
source_filename: soracom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/soracom-analysis-query-api-openapi.yml, openapi/soracom-auth-api-openapi.yml,\n  openapi/soracom-batch-api-openapi.yml, openapi/soracom-billing-api-openapi.yml, openapi/soracom-event-handler-api-openapi.yml,\n  openapi/soracom-group-api-openapi.yml, openapi/soracom-harvest-api-openapi.yml, openapi/soracom-inventory-api-openapi.yml,\n  openapi/soracom-lagoon-api-openapi.yml, openapi/soracom-lorawan-api-openapi.yml, openapi/soracom-napter-api-openapi.yml,\n  openapi/soracom-platform-api-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Soracom-API-Key\n  description: |-\n    API key for authentication. Obtain this from the Soracom User Console or via the Auth API.\n    Required in combination with an API token for all authenticated requests.\n  sources:\n  - openapi/soracom-analysis-query-api-openapi.yml\n  - openapi/soracom-auth-api-openapi.yml\n\
  \  - openapi/soracom-batch-api-openapi.yml\n  - openapi/soracom-billing-api-openapi.yml\n  - openapi/soracom-event-handler-api-openapi.yml\n  - openapi/soracom-group-api-openapi.yml\n  - openapi/soracom-harvest-api-openapi.yml\n  - openapi/soracom-inventory-api-openapi.yml\n  - openapi/soracom-lagoon-api-openapi.yml\n  - openapi/soracom-lorawan-api-openapi.yml\n  - openapi/soracom-napter-api-openapi.yml\n  - openapi/soracom-platform-api-openapi.yml\n  - openapi/soracom-sigfox-api-openapi.yml\n  - openapi/soracom-sim-api-openapi.yml\n  - openapi/soracom-soracam-api-openapi.yml\n  - openapi/soracom-stats-api-openapi.yml\n  - openapi/soracom-vpg-api-openapi.yml\n- name: api_token\n  type: apiKey\n  in: header\n  parameter: X-Soracom-Token\n  description: |-\n    API token for authentication. This token has an expiration time and must be refreshed periodically.\n    Required in combination with an API key for all authenticated requests.\n  sources:\n  - openapi/soracom-analysis-query-api-openapi.yml\n\
  \  - openapi/soracom-auth-api-openapi.yml\n  - openapi/soracom-batch-api-openapi.yml\n  - openapi/soracom-billing-api-openapi.yml\n  - openapi/soracom-event-handler-api-openapi.yml\n  - openapi/soracom-group-api-openapi.yml\n  - openapi/soracom-harvest-api-openapi.yml\n  - openapi/soracom-inventory-api-openapi.yml\n  - openapi/soracom-lagoon-api-openapi.yml\n  - openapi/soracom-lorawan-api-openapi.yml\n  - openapi/soracom-napter-api-openapi.yml\n  - openapi/soracom-platform-api-openapi.yml\n  - openapi/soracom-sigfox-api-openapi.yml\n  - openapi/soracom-sim-api-openapi.yml\n  - openapi/soracom-soracam-api-openapi.yml\n  - openapi/soracom-stats-api-openapi.yml\n  - openapi/soracom-vpg-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/authentication/soracom-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- IoT
- Cellular
- LPWAN
- SIM
- LoRaWAN
- Sigfox
- MVNO
- Connectivity
- Edge
- Japan
---
