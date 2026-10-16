---
anonymous_access: false
api_key_in: []
api_specs:
- filename: picomes-openapi-generated.yml
  format: yaml
  label: Picomes API
  slug: picomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picomes/refs/heads/main/openapi/_ae-authored/picomes-openapi-generated.yml
auth_types: []
description: Authentication schemes for Picomes API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Picomes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Picomes declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Picomes
provider_slug: picomes
scheme_count: 1
schemes:
- evidence: 'To authenticate API requests, include your token in the x-pico-api-org header: x-pico-api-org: your-api-token'
  header: x-pico-api-org
  how_to_obtain: API tokens are generated on a per-instance basis. To request an authentication token for your Pico instance, please contact support.
  location: header
  name: x-pico-api-org
  type: apiKey
slug: picomes-authentication
source_filename: picomes-authentication.yml
source_heading: Authentication Profile
source_url: https://apidocs.picomes.com/guides/authentication/index.html
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://apidocs.picomes.com/guides/authentication/index.html\nsources:\n- https://apidocs.picomes.com/guides/authentication/index.html\n- https://apidocs.picomes.com/types/inputs/oauth-config-input/index.html\ndescription: Authentication schemes for Picomes API\nschemes:\n- type: apiKey\n  name: x-pico-api-org\n  evidence: 'To authenticate API requests, include your token in the x-pico-api-org header: x-pico-api-org: your-api-token'\n  location: header\n  header: x-pico-api-org\n  how_to_obtain: API tokens are generated on a per-instance basis. To request an authentication token for your Pico instance, please contact support.\ndocs: https://apidocs.picomes.com/guides/authentication/index.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picomes/refs/heads/main/authentication/picomes-authentication.yml
summary_line: 1 scheme
tags:
- Manufacturing
- MES
- IoT
- ErrorProofing
- Software
---
