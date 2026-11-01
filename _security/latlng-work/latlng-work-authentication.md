---
anonymous_access: false
api_key_in: []
api_specs:
- filename: latlng-work-geocoding-api-openapi.yml
  format: yaml
  label: latlng-work Geocoding API
  slug: latlng-work-geocoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latlng-work/openapi/latlng-work-geocoding-api-openapi.yml
- filename: latlng-work-places-api-openapi.yml
  format: yaml
  label: latlng-work Places API
  slug: latlng-work-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latlng-work/openapi/latlng-work-places-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Latlng Work Authentication
name_suffix: Authentication
oauth_flows: []
overview: latlng-work declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: latlng-work
provider_slug: latlng-work
scheme_count: 2
schemes:
- description: Server Key, used for all APIs, keep secret.
  in: header
  name: X-Api-Key
  type: apiKey
- description: Maps Key, safe for client-side, can be domain-restricted.
  in: query
  name: api_key
  type: apiKey
slug: latlng-work-authentication
source_filename: latlng-work-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: \"https://www.latlng.work/docs\"\nschemes:\n  - type: apiKey\n    in: header\n    name: X-Api-Key\n    description: Server Key, used for all APIs, keep secret.\n  - type: apiKey\n    in: query\n    name: api_key\n    description: Maps Key, safe for client-side, can be domain-restricted.\n"
source_yaml_url: https://artifacts.apis.io/latlng-work/authentication/latlng-work-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Geocoding
- Mapping
- API
- Location
---
