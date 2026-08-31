---
api_key_in:
- header
api_specs:
- filename: realestateapi-avm-api-openapi.yml
  format: yaml
  label: RealEstateAPI AVM API
  slug: realestateapi-avm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realestateapi/refs/heads/main/openapi/realestateapi-avm-api-openapi.yml
- filename: realestateapi-comparables-api-openapi.yml
  format: yaml
  label: RealEstateAPI Comparables API
  slug: realestateapi-comparables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realestateapi/refs/heads/main/openapi/realestateapi-comparables-api-openapi.yml
- filename: realestateapi-liens-api-openapi.yml
  format: yaml
  label: RealEstateAPI Liens API
  slug: realestateapi-liens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realestateapi/refs/heads/main/openapi/realestateapi-liens-api-openapi.yml
- filename: realestateapi-mls-api-openapi.yml
  format: yaml
  label: RealEstateAPI MLS API
  slug: realestateapi-mls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realestateapi/refs/heads/main/openapi/realestateapi-mls-api-openapi.yml
- filename: realestateapi-parcel-api-openapi.yml
  format: yaml
  label: RealEstateAPI Parcel API
  slug: realestateapi-parcel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realestateapi/refs/heads/main/openapi/realestateapi-parcel-api-openapi.yml
- filename: realestateapi-property-detail-api-openapi.yml
  format: yaml
  label: RealEstateAPI Property Detail API
  slug: realestateapi-property-detail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realestateapi/refs/heads/main/openapi/realestateapi-property-detail-api-openapi.yml
- filename: realestateapi-property-search-api-openapi.yml
  format: yaml
  label: RealEstateAPI Property Search API
  slug: realestateapi-property-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realestateapi/refs/heads/main/openapi/realestateapi-property-search-api-openapi.yml
- filename: realestateapi-skip-trace-api-openapi.yml
  format: yaml
  label: RealEstateAPI Skip Trace API
  slug: realestateapi-skip-trace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realestateapi/refs/heads/main/openapi/realestateapi-skip-trace-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Realestateapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: RealEstateAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RealEstateAPI
provider_slug: realestateapi
scheme_count: 1
schemes:
- description: RealEstateAPI account API key.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/realestateapi-openapi.yml
  type: apiKey
slug: realestateapi-authentication
source_filename: realestateapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/realestateapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: RealEstateAPI account API key.\n  sources:\n  - openapi/realestateapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realestateapi/refs/heads/main/authentication/realestateapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Real-Estate
- Property Data
- MLS
- Valuation
- Geospatial
- Skip Tracing
- Prop-Tech
---
