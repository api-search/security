---
api_key_in:
- header
- query
api_specs:
- filename: openchargemap-comment-api-openapi.yml
  format: yaml
  label: Open Charge Map Comment API
  slug: openchargemap-comment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-openchargemap/refs/heads/main/openapi/openchargemap-comment-api-openapi.yml
- filename: openchargemap-mediaitem-api-openapi.yml
  format: yaml
  label: Open Charge Map Mediaitem API
  slug: openchargemap-mediaitem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-openchargemap/refs/heads/main/openapi/openchargemap-mediaitem-api-openapi.yml
- filename: openchargemap-openapi-api-openapi.yml
  format: yaml
  label: Open Charge Map Openapi API
  slug: openchargemap-openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-openchargemap/refs/heads/main/openapi/openchargemap-openapi-api-openapi.yml
- filename: openchargemap-poi-api-openapi.yml
  format: yaml
  label: Open Charge Map Poi API
  slug: openchargemap-poi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-openchargemap/refs/heads/main/openapi/openchargemap-poi-api-openapi.yml
- filename: openchargemap-profile-api-openapi.yml
  format: yaml
  label: Open Charge Map Profile API
  slug: openchargemap-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-openchargemap/refs/heads/main/openapi/openchargemap-profile-api-openapi.yml
- filename: openchargemap-referencedata-api-openapi.yml
  format: yaml
  label: Open Charge Map Referencedata API
  slug: openchargemap-referencedata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-openchargemap/refs/heads/main/openapi/openchargemap-referencedata-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openchargemap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Charge Map secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Open Charge Map
provider_slug: api-evangelist-openchargemap
scheme_count: 3
schemes:
- description: API Key supplied as query string parameter
  in: query
  name: APIKeyQueryString
  parameter: key
  sources:
  - openapi/openapi.yaml
  type: apiKey
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/openapi.yaml
  type: apiKey
- name: UserAuthentication
  scheme: bearer
  sources:
  - openapi/openapi.yaml
  type: http
slug: openchargemap-authentication
source_filename: openchargemap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: APIKeyQueryString\n  type: apiKey\n  in: query\n  parameter: key\n  description: API Key supplied as query string parameter\n  sources:\n  - openapi/openapi.yaml\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/openapi.yaml\n- name: UserAuthentication\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-openchargemap/refs/heads/main/authentication/openchargemap-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Electric Vehicles
- EV Charging
- Charging Stations
- Points of Interest
- Open Data
- Geospatial
- Transportation
- Clean Energy
- Crowdsourced
- Registry
---
