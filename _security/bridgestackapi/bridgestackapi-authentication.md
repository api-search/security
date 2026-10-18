---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bridgestackapi-bridgestackapi-api-api-openapi.yml
  format: yaml
  label: BridgeStackAPI BridgeStackAPI API
  slug: bridgestackapi-bridgestackapi-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridgestackapi/refs/heads/main/openapi/bridgestackapi-bridgestackapi-api-api-openapi.yml
auth_types: []
description: Authentication schemes for BridgeStackAPI
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bridgestackapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: BridgeStackAPI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BridgeStackAPI
provider_slug: bridgestackapi
scheme_count: 1
schemes:
- evidence: Send the BridgeStackAPI key in every request using the x-api-key header.
  header: x-api-key
  location: header
  name: x-api-key
  type: apiKey
slug: bridgestackapi-authentication
source_filename: bridgestackapi-authentication.yml
source_heading: Authentication Profile
source_url: https://www.bridgestackapi.com/docs/getting-started/authentication
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.bridgestackapi.com/docs/getting-started/authentication\nsources:\n- https://www.bridgestackapi.com/docs/getting-started/authentication\n- https://www.bridgestackapi.com/docs/api-reference#auth\n- https://www.bridgestackapi.com/docs/api-reference\n- https://www.bridgestackapi.com/docs/core-concepts\ndescription: Authentication schemes for BridgeStackAPI\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: Send the BridgeStackAPI key in every request using the x-api-key header.\n  location: header\n  header: x-api-key\ndocs: https://www.bridgestackapi.com/docs/getting-started/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridgestackapi/refs/heads/main/authentication/bridgestackapi-authentication.yml
summary_line: 1 scheme
tags:
- API Gateway
- Usage Control
- B2B SaaS
- External APIs
---
