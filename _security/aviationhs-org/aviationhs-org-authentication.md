---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aviationhs-org-aircraft-api-openapi.yml
  format: yaml
  label: AviationHS Aircraft API
  slug: aviationhs-org-aircraft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviationhs-org/openapi/aviationhs-org-aircraft-api-openapi.yml
- filename: aviationhs-org-airports-api-openapi.yml
  format: yaml
  label: AviationHS Airports API
  slug: aviationhs-org-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviationhs-org/openapi/aviationhs-org-airports-api-openapi.yml
- filename: aviationhs-org-runway-api-openapi.yml
  format: yaml
  label: AviationHS Runway API
  slug: aviationhs-org-runway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviationhs-org/openapi/aviationhs-org-runway-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AviationHS Authentication
name_suffix: Authentication
oauth_flows: []
overview: AviationHS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AviationHS
provider_slug: aviationhs-org
scheme_count: 1
schemes:
- description: OAuth 2.1 required for write tools (create_trip_request)
  flows: {}
  type: oauth2
slug: aviationhs-org-authentication
source_filename: aviationhs-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://aviationhs.org/developers/\nschemes:\n  - type: oauth2\n    description: OAuth 2.1 required for write tools (create_trip_request)\n    flows: {}\n"
source_yaml_url: https://artifacts.apis.io/aviationhs-org/authentication/aviationhs-org-authentication.yml
summary_line: 1 scheme
tags:
- Private-Jet
- Charter
- Aviation
- QuoteEngine
- MCP
---
