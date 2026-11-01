---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ivalt-openapi-generated.yml
  format: yaml
  label: iVALT API
  slug: ivalt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivalt/openapi/_ae-authored/ivalt-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ivalt Authentication
name_suffix: Authentication
oauth_flows: []
overview: iVALT declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: iVALT
provider_slug: ivalt
scheme_count: 1
schemes:
- evidence: API key required in the header.
  header: x-api-key
  location: header
  name: ApiKeyAuth
  type: apiKey
slug: ivalt-authentication
source_filename: ivalt-authentication.yml
source_heading: Authentication Profile
source_url: https://api-docs.ivalt.com/products/authentication/auth_apis.md
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api-docs.ivalt.com/products/authentication/auth_apis.md\nsources:\n- https://api-docs.ivalt.com/products/authentication/auth_apis.md\n- https://api-docs.ivalt.com/products/authentication.md\n- https://api-docs.ivalt.com/products/getting-started.md\nschemes:\n- type: apiKey\n  name: ApiKeyAuth\n  evidence: API key required in the header.\n  location: header\n  header: x-api-key\ndocs: https://api-docs.ivalt.com/products/authentication/auth_apis.md\n"
source_yaml_url: https://artifacts.apis.io/ivalt/authentication/ivalt-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Identity
- Security
- HumanAuthority
---
