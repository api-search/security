---
api_key_in: []
api_specs:
- filename: gemfury-gemfury-api-openapi.yml
  format: yaml
  label: Gemfury Developer API
  slug: gemfury-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemfury/refs/heads/main/openapi/gemfury-gemfury-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gemfury Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gemfury secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gemfury
provider_slug: gemfury
scheme_count: 1
schemes:
- description: API token obtained from the Gemfury dashboard
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gemfury-gemfury-api-openapi.yml
  type: http
slug: gemfury-authentication
source_filename: gemfury-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gemfury-gemfury-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API token obtained from the Gemfury dashboard\n  sources:\n  - openapi/gemfury-gemfury-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gemfury/refs/heads/main/authentication/gemfury-authentication.yml
summary_line: http · 1 scheme
tags:
- Package Repository
- Private Packages
- Gem
- npm
- PyPI
- Composer
- NuGet
- Go Modules
- Maven
- DEB
- RPM
- Bower
- Rust Crates
- Developer Tools
---
