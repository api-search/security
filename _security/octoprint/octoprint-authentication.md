---
anonymous_access: false
api_key_in: []
api_specs:
- filename: octoprint-openapi-generated.yml
  format: yaml
  label: OctoPrint API
  slug: octoprint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octoprint/openapi/_ae-authored/octoprint-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Octoprint Authentication
name_suffix: Authentication
oauth_flows: []
overview: OctoPrint declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OctoPrint
provider_slug: octoprint
scheme_count: 1
schemes:
- description: System-wide API key for authenticating requests.
  in: header
  name: apikey
  type: apiKey
slug: octoprint-authentication
source_filename: octoprint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://docs.octoprint.org/en/main/api/settings.html\nschemes:\n  - type: apiKey\n    name: apikey\n    in: header\n    description: System-wide API key for authenticating requests.\n"
source_yaml_url: https://artifacts.apis.io/octoprint/authentication/octoprint-authentication.yml
summary_line: 1 scheme
tags:
- Company
- 3D Printing
- Open Source
- IoT
- Maker
---
