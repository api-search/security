---
api_key_in: []
api_specs:
- filename: car-api-account-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Account API
  slug: car-api-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-account-api-openapi.yml
- filename: car-api-auth-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Auth API
  slug: car-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-auth-api-openapi.yml
- filename: car-api-bodies-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Bodies API
  slug: car-api-bodies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-bodies-api-openapi.yml
- filename: car-api-colors-exterior-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Colors (Exterior) API
  slug: car-api-colors-exterior-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-colors-exterior-api-openapi.yml
- filename: car-api-colors-interior-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Colors (Interior) API
  slug: car-api-colors-interior-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-colors-interior-api-openapi.yml
- filename: car-api-data-feeds-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Data Feeds API
  slug: car-api-data-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-data-feeds-api-openapi.yml
- filename: car-api-engines-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Engines API
  slug: car-api-engines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-engines-api-openapi.yml
- filename: car-api-makes-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Makes API
  slug: car-api-makes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-makes-api-openapi.yml
- filename: car-api-mileages-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Mileages API
  slug: car-api-mileages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-mileages-api-openapi.yml
- filename: car-api-models-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Models API
  slug: car-api-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-models-api-openapi.yml
- filename: car-api-trims-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Trims API
  slug: car-api-trims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-trims-api-openapi.yml
- filename: car-api-vehicle-attributes-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Vehicle Attributes API
  slug: car-api-vehicle-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-vehicle-attributes-api-openapi.yml
- filename: car-api-vin-decoder-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Vin Decoder API
  slug: car-api-vin-decoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-vin-decoder-api-openapi.yml
- filename: car-api-years-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Years API
  slug: car-api-years-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-years-api-openapi.yml
- filename: car-api-authentication-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Authentication API
  slug: car-api-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-authentication-api-openapi.yml
- filename: car-api-vehicles-api-openapi.yml
  format: yaml
  label: Car API (carapi.app) Vehicles API
  slug: car-api-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-vehicles-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Car Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Car API (carapi.app) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Car API (carapi.app)
provider_slug: car-api
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/car-api-openapi-original.yml
  type: http
slug: car-api-authentication
source_filename: car-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/car-api-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/car-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/authentication/car-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Automobiles
- Automotive Data
- Cars
- License Plate Decoder
- OBD-II
- Power Sports
- Vehicle API
- Vehicle Specifications
- Vehicles
- VIN Decoder
---
