---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ignav-com-airports-api-openapi.yml
  format: yaml
  label: ignav-com Airports API
  slug: ignav-com-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ignav-com/openapi/ignav-com-airports-api-openapi.yml
- filename: ignav-com-fares-api-openapi.yml
  format: yaml
  label: ignav-com Fares API
  slug: ignav-com-fares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ignav-com/openapi/ignav-com-fares-api-openapi.yml
- filename: ignav-com-health-api-openapi.yml
  format: yaml
  label: ignav-com Health API
  slug: ignav-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ignav-com/openapi/ignav-com-health-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ignav Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ignav-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ignav-com
provider_slug: ignav-com
scheme_count: 1
schemes:
- description: API key provided in X-Api-Key header.
  in: header
  name: X-Api-Key
  type: apiKey
slug: ignav-com-authentication
source_filename: ignav-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://ignav.com/docs/authentication\nschemes:\n  - type: apiKey\n    name: X-Api-Key\n    in: header\n    description: API key provided in X-Api-Key header.\n"
source_yaml_url: https://artifacts.apis.io/ignav-com/authentication/ignav-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Flight
- Travel
- API
- Pricing
- Data
---
