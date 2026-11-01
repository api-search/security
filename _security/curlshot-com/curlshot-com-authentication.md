---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Curlshot Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: curlshot-com declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: curlshot-com
provider_slug: curlshot-com
scheme_count: 3
schemes:
- description: Access key sent in header.
  in: header
  name: X-Access-Key
  type: apiKey
- description: Access key as query parameter.
  in: query
  name: access_key
  type: apiKey
- bearerFormat: JWT
  description: Bearer token authentication.
  scheme: bearer
  type: http
slug: curlshot-com-authentication
source_filename: curlshot-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://curlshot.com/docs/authentication.md\nschemes:\n  - type: apiKey\n    name: X-Access-Key\n    in: header\n    description: Access key sent in header.\n  - type: apiKey\n    name: access_key\n    in: query\n    description: Access key as query parameter.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token authentication.\n"
source_yaml_url: https://artifacts.apis.io/curlshot-com/authentication/curlshot-com-authentication.yml
summary_line: 3 schemes
tags:
- Screenshot
- API
- Web
- Automation
- DeveloperTools
---
