---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bright-mls-auth-api-openapi.yml
  format: yaml
  label: Bright MLS Auth API
  slug: bright-mls-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-auth-api-openapi.yml
- filename: bright-mls-listing-api-openapi.yml
  format: yaml
  label: Bright MLS Listing API
  slug: bright-mls-listing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-listing-api-openapi.yml
- filename: bright-mls-manifests-api-openapi.yml
  format: yaml
  label: Bright MLS Manifests API
  slug: bright-mls-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-manifests-api-openapi.yml
- filename: bright-mls-user-api-openapi.yml
  format: yaml
  label: Bright MLS User API
  slug: bright-mls-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-user-api-openapi.yml
- filename: bright-mls-data-hub-api-openapi.yml
  format: yaml
  label: Bright MLS Data Hub API
  slug: bright-mls-data-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/openapi/bright-mls-data-hub-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Bright Mls Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bright MLS secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bright MLS
provider_slug: bright-mls
scheme_count: 3
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/bright-mls-data-hub-ingestion-service-openapi.json
  type: apiKey
- in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/bright-mls-datalake-distribution-service-openapi.json
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/bright-mls-manifest-services-openapi.json
  type: apiKey
slug: bright-mls-authentication
source_filename: bright-mls-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/bright-mls-data-hub-ingestion-service-openapi.json, openapi/bright-mls-datalake-distribution-service-openapi.json,\n  openapi/bright-mls-manifest-services-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/bright-mls-data-hub-ingestion-service-openapi.json\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/bright-mls-datalake-distribution-service-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/bright-mls-manifest-services-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-mls/refs/heads/main/authentication/bright-mls-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Real Estate
- MLS
- RESO
- OData
- Listings
- Property Data
---
