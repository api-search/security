---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Pict Rs Authentication
name_suffix: Authentication
oauth_flows: []
overview: pict-rs declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: pict-rs
provider_slug: pict-rs
scheme_count: 3
schemes:
- description: API tokens must be prepended with "token "
  in: header
  name: Authorization
  type: apiKey
- description: Basic HTTP authentication
  type: basic
- description: Sudo API request as the user provided as the key (admin required)
  in: header
  name: Sudo
  type: apiKey
slug: pict-rs-authentication
source_filename: pict-rs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: https://git.asonix.dog/swagger.v1.json\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: API tokens must be prepended with \"token \"\n  - type: basic\n    description: Basic HTTP authentication\n  - type: apiKey\n    name: Sudo\n    in: header\n    description: Sudo API request as the user provided as the key (admin required)\n"
source_yaml_url: https://artifacts.apis.io/pict-rs/authentication/pict-rs-authentication.yml
summary_line: 3 schemes
tags:
- Image Hosting
- Rust
- Open Source
- API
- Self-hosted
---
