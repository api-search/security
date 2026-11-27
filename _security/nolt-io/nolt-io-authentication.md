---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Nolt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nolt declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Nolt
provider_slug: nolt-io
scheme_count: 3
schemes:
- description: API key provided in board settings under "APIs" section.
  in: header
  name: apikey
  type: apiKey
- description: SSO type (optional for SSO user creation).
  in: header
  name: ssotype
  type: apiKey
- description: SSO user ID (optional for SSO user creation).
  in: header
  name: ssoid
  type: apiKey
slug: nolt-io-authentication
source_filename: nolt-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: searched\nsource: https://nolt.io/docs/publicapi/authentication/\nschemes:\n  - type: apiKey\n    name: apikey\n    in: header\n    description: API key provided in board settings under \"APIs\" section.\n  - type: apiKey\n    name: ssotype\n    in: header\n    description: SSO type (optional for SSO user creation).\n  - type: apiKey\n    name: ssoid\n    in: header\n    description: SSO user ID (optional for SSO user creation).\n"
source_yaml_url: https://artifacts.apis.io/nolt-io/authentication/nolt-io-authentication.yml
summary_line: 3 schemes
tags:
- Feedback Management
- Product Roadmap
- User Research
---
