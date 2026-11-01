---
anonymous_access: false
api_key_in: []
api_specs:
- filename: iplocate-openapi.yml
  format: yaml
  label: IPLocate API
  slug: iplocate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iplocate/openapi/iplocate-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Iplocate Authentication
name_suffix: Authentication
oauth_flows: []
overview: IPLocate (formerly GeoIPs) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: IPLocate (formerly GeoIPs)
provider_slug: iplocate
scheme_count: 1
schemes:
- description: Provide your API key as a query parameter `apikey`.
  in: query
  name: API Key
  type: apiKey
slug: iplocate-authentication
source_filename: iplocate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: searched\nsource: https://www.iplocate.io/docs/getting-started/authentication\nschemes:\n  - type: apiKey\n    name: API Key\n    in: query\n    description: Provide your API key as a query parameter `apikey`.\n"
source_yaml_url: https://artifacts.apis.io/iplocate/authentication/iplocate-authentication.yml
summary_line: 1 scheme
tags:
- Company
- IP Geolocation
- Threat Detection
- Privacy
- API
- Data
---
