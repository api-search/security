---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hashdit-address-intelligence-api-openapi.yml
  format: yaml
  label: HashDit Address Intelligence API
  slug: hashdit-address-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashdit/openapi/hashdit-address-intelligence-api-openapi.yml
- filename: hashdit-domain-security-api-openapi.yml
  format: yaml
  label: HashDit Domain Security API
  slug: hashdit-domain-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashdit/openapi/hashdit-domain-security-api-openapi.yml
- filename: hashdit-signature-security-api-openapi.yml
  format: yaml
  label: HashDit Signature Security API
  slug: hashdit-signature-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashdit/openapi/hashdit-signature-security-api-openapi.yml
- filename: hashdit-simulation-api-openapi.yml
  format: yaml
  label: HashDit Simulation API
  slug: hashdit-simulation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashdit/openapi/hashdit-simulation-api-openapi.yml
- filename: hashdit-token-security-api-openapi.yml
  format: yaml
  label: HashDit Token Security API
  slug: hashdit-token-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashdit/openapi/hashdit-token-security-api-openapi.yml
- filename: hashdit-transaction-security-api-openapi.yml
  format: yaml
  label: HashDit Transaction Security API
  slug: hashdit-transaction-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashdit/openapi/hashdit-transaction-security-api-openapi.yml
auth_types: []
description: HashDit API authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: HashDit Authentication
name_suffix: Authentication
oauth_flows: []
overview: HashDit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: HashDit
provider_slug: hashdit
scheme_count: 1
schemes:
- evidence: '**X-API-KEY** `string` *required* Your HashDit API key.'
  header: X-API-KEY
  location: header
  name: X-API-KEY
  type: apiKey
slug: hashdit-authentication
source_filename: hashdit-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.hashdit.io/api-reference/endpoint/token-security.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.hashdit.io/api-reference/endpoint/token-security.md\nsources:\n- https://docs.hashdit.io/api-reference/endpoint/token-security.md\n- https://docs.hashdit.io/api-reference/endpoint/solana-token-security.md\n- https://docs.hashdit.io/api-reference/endpoint/token-approval-security.md\n- https://docs.hashdit.io/blog/2024-05-15/2024-05-15.md\ndescription: HashDit API authentication\nschemes:\n- type: apiKey\n  name: X-API-KEY\n  evidence: '**X-API-KEY** `string` *required* Your HashDit API key.'\n  location: header\n  header: X-API-KEY\ndocs: https://docs.hashdit.io/api-reference/endpoint/token-security.md\n"
source_yaml_url: https://artifacts.apis.io/hashdit/authentication/hashdit-authentication.yml
summary_line: 1 scheme
tags:
- Crypto Security
- Scam Protection
- Token Scanner
- Web3 Tools
- Monitoring Platform
---
