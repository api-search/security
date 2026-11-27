---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cryptoamlpolicy-com-enquiry-api-openapi.yml
  format: yaml
  label: Crypto AML Policy Enquiry API
  slug: cryptoamlpolicy-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptoamlpolicy-com/openapi/cryptoamlpolicy-com-enquiry-api-openapi.yml
- filename: cryptoamlpolicy-com-mcp-api-openapi.yml
  format: yaml
  label: Crypto AML Policy MCP API
  slug: cryptoamlpolicy-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptoamlpolicy-com/openapi/cryptoamlpolicy-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Crypto AML Policy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crypto AML Policy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crypto AML Policy
provider_slug: cryptoamlpolicy-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/cryptoamlpolicy-com-openapi.json
  type: http
slug: cryptoamlpolicy-com-authentication
source_filename: cryptoamlpolicy-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/cryptoamlpolicy-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/cryptoamlpolicy-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cryptoamlpolicy-com/authentication/cryptoamlpolicy-com-authentication.yml
summary_line: http · 1 scheme
tags:
- AML
- Cryptocurrency
- Policy
- Templates
- Compliance
---
