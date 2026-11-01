---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Sonarr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sonarr declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Sonarr
provider_slug: sonarr
scheme_count: 2
schemes:
- description: Apikey passed as header
  in: header
  name: X-Api-Key
  type: apiKey
- description: Apikey passed as query parameter
  in: query
  name: apikey
  type: apiKey
slug: sonarr-authentication
source_filename: sonarr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource:\n  - url: https://raw.githubusercontent.com/Sonarr/Sonarr/develop/src/Sonarr.Api.V5/openapi.json\n    type: openapi\nschemes:\n  - type: apiKey\n    name: X-Api-Key\n    in: header\n    description: Apikey passed as header\n  - type: apiKey\n    name: apikey\n    in: query\n    description: Apikey passed as query parameter\n"
source_yaml_url: https://artifacts.apis.io/sonarr/authentication/sonarr-authentication.yml
summary_line: 2 schemes
tags:
- Company
- PVR
- TV
- Usenet
- Torrent
- Automation
---
