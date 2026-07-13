---
api_key_in:
- header
- query
api_specs:
- filename: demandbase-api-openapi.yml
  format: yaml
  label: Demandbase API
  slug: demandbase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-api-openapi.yml
- filename: demandbase-real-time-identification-openapi.yml
  format: yaml
  label: Demandbase Real-Time Identification API
  slug: demandbase-real-time-identification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-real-time-identification-openapi.yml
- filename: demandbase-advertising-openapi.yml
  format: yaml
  label: Demandbase Advertising API
  slug: demandbase-advertising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-advertising-openapi.yml
- filename: demandbase-engagement-openapi.yml
  format: yaml
  label: Demandbase Engagement API
  slug: demandbase-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-engagement-openapi.yml
- filename: demandbase-account-list-openapi.yml
  format: yaml
  label: Demandbase Account List API
  slug: demandbase-account-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-account-list-openapi.yml
- filename: demandbase-b2b-data-openapi.yml
  format: yaml
  label: Demandbase B2B Data API
  slug: demandbase-b2b-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-b2b-data-openapi.yml
- filename: demandbase-ip-openapi.yml
  format: yaml
  label: Demandbase IP API
  slug: demandbase-ip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-ip-openapi.yml
- filename: demandbase-admin-openapi.yml
  format: yaml
  label: Demandbase Admin API
  slug: demandbase-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-admin-openapi.yml
- filename: demandbase-data-export-openapi.yml
  format: yaml
  label: Demandbase Data Export API
  slug: demandbase-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-data-export-openapi.yml
- filename: demandbase-data-import-openapi.yml
  format: yaml
  label: Demandbase Data Import API
  slug: demandbase-data-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-data-import-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Demandbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Demandbase secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Demandbase
provider_slug: demandbase
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token for API access
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/demandbase-account-list-openapi.yml
  - openapi/demandbase-admin-openapi.yml
  - openapi/demandbase-advertising-openapi.yml
  - openapi/demandbase-data-export-openapi.yml
  - openapi/demandbase-data-import-openapi.yml
  - openapi/demandbase-engagement-openapi.yml
  type: http
- description: API key provided as a bearer token in the Authorization header
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/demandbase-api-openapi.yml
  - openapi/demandbase-b2b-data-openapi.yml
  type: apiKey
- description: Demandbase API key passed as query parameter
  in: query
  name: apiKeyAuth
  parameter: key
  sources:
  - openapi/demandbase-ip-openapi.yml
  - openapi/demandbase-real-time-identification-openapi.yml
  type: apiKey
slug: demandbase-authentication
source_filename: demandbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/demandbase-account-list-openapi.yml, openapi/demandbase-admin-openapi.yml, openapi/demandbase-advertising-openapi.yml,\n  openapi/demandbase-api-openapi.yml, openapi/demandbase-b2b-data-openapi.yml, openapi/demandbase-data-export-openapi.yml,\n  openapi/demandbase-data-import-openapi.yml, openapi/demandbase-engagement-openapi.yml, openapi/demandbase-ip-openapi.yml,\n  openapi/demandbase-real-time-identification-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token for API access\n  sources:\n  - openapi/demandbase-account-list-openapi.yml\n  - openapi/demandbase-admin-openapi.yml\n  - openapi/demandbase-advertising-openapi.yml\n  - openapi/demandbase-data-export-openapi.yml\n  - openapi/demandbase-data-import-openapi.yml\n  - openapi/demandbase-engagement-openapi.yml\n\
  - name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key provided as a bearer token in the Authorization header\n  sources:\n  - openapi/demandbase-api-openapi.yml\n  - openapi/demandbase-b2b-data-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  description: Demandbase API key passed as query parameter\n  sources:\n  - openapi/demandbase-ip-openapi.yml\n  - openapi/demandbase-real-time-identification-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/authentication/demandbase-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Account-Based Marketing
- Advertising
- AI Agents
- B2B Marketing
- Data Enrichment
- Intent Data
- Personalization
- Sales Intelligence
---
