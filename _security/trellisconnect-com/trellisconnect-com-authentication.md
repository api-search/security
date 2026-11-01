---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Trellisconnect Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trellis declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Trellis
provider_slug: trellisconnect-com
scheme_count: 3
schemes:
- description: Client identifier for authentication.
  in: header
  name: X-API-Client-Id
  type: apiKey
- description: Secret key for server-to-server authentication.
  in: header
  name: X-API-Secret-Key
  type: apiKey
- description: Temporary access key for client-side usage, limited time.
  in: header
  name: X-API-Temporary-Access-Key
  type: apiKey
slug: trellisconnect-com-authentication
source_filename: trellisconnect-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://docs.trellisconnect.com/trellis/1.1.0\nschemes:\n  - type: apiKey\n    name: X-API-Client-Id\n    in: header\n    description: Client identifier for authentication.\n  - type: apiKey\n    name: X-API-Secret-Key\n    in: header\n    description: Secret key for server-to-server authentication.\n  - type: apiKey\n    name: X-API-Temporary-Access-Key\n    in: header\n    description: Temporary access key for client-side usage, limited time.\n"
source_yaml_url: https://artifacts.apis.io/trellisconnect-com/authentication/trellisconnect-com-authentication.yml
summary_line: 3 schemes
tags:
- Insurance
- Car Insurance
- Licensed Agency
- AI Assistants
---
