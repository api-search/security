---
anonymous_access: false
api_key_in: []
api_specs:
- filename: shotkit-net-openapi-generated.yml
  format: yaml
  label: shotkit-net API
  slug: shotkit-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shotkit-net/openapi/_ae-authored/shotkit-net-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Shotkit Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: shotkit-net declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: shotkit-net
provider_slug: shotkit-net
scheme_count: 3
schemes:
- description: Access key for identifying workspace.
  in: header
  name: X-Access-Key
  type: apiKey
- description: Access key as query parameter.
  in: query
  name: access_key
  type: apiKey
- description: Signed requests using secret key (signature in query or X-Signature header).
  scheme: hmac
  type: http
slug: shotkit-net-authentication
source_filename: shotkit-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://shotkit.net/docs/authentication.md\nschemes:\n  - type: apiKey\n    name: X-Access-Key\n    in: header\n    description: Access key for identifying workspace.\n  - type: apiKey\n    name: access_key\n    in: query\n    description: Access key as query parameter.\n  - type: http\n    scheme: hmac\n    description: Signed requests using secret key (signature in query or X-Signature header).\n"
source_yaml_url: https://artifacts.apis.io/shotkit-net/authentication/shotkit-net-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Screenshot
- API
- Web
- Automation
---
