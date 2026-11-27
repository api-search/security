---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Everfox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Everfox declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Everfox
provider_slug: everfox
scheme_count: 2
schemes:
- description: API Key required for every call.
  in: header
  name: x-api-key
  type: apiKey
- description: AWS Signature Version 4 used for actions after the initial API call in the Async API.
  name: sigv4
  type: custom
slug: everfox-authentication
source_filename: everfox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://cdr.everfox.com/api/instant/documentation\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: API Key required for every call.\n  - type: custom\n    name: sigv4\n    description: AWS Signature Version 4 used for actions after the initial API call in the Async API.\n"
source_yaml_url: https://artifacts.apis.io/everfox/authentication/everfox-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Security
- Data
- Cloud
- Government
---
