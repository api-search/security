---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Lawdiver Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: LawDiver declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: LawDiver
provider_slug: lawdiver-com
scheme_count: 4
schemes:
- description: Bearer token, format "Bearer <key>"
  in: header
  name: Authorization
  type: apiKey
- description: API key header
  in: header
  name: X-API-Key
  type: apiKey
- description: Optional API key label header
  in: header
  name: lawdiver_api_key
  type: apiKey
- description: API key as query parameter
  in: query
  name: lawdiver_api_key
  type: apiKey
slug: lawdiver-com-authentication
source_filename: lawdiver-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://lawdiver.com/docs/api\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer token, format \"Bearer <key>\"\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key header\n  - type: apiKey\n    name: lawdiver_api_key\n    in: header\n    description: Optional API key label header\n  - type: apiKey\n    name: lawdiver_api_key\n    in: query\n    description: API key as query parameter\n"
source_yaml_url: https://artifacts.apis.io/lawdiver-com/authentication/lawdiver-com-authentication.yml
summary_line: 4 schemes
tags:
- Company
- LegalTech
- LegalResearch
- API
- Free
---
