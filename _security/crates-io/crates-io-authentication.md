---
api_key_in:
- header
api_specs:
- filename: crates-io-config-api-openapi.yml
  format: yaml
  label: crates.io Config API
  slug: crates-io-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/openapi/crates-io-config-api-openapi.yml
- filename: crates-io-crates-api-openapi.yml
  format: yaml
  label: crates.io Crates API
  slug: crates-io-crates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/openapi/crates-io-crates-api-openapi.yml
- filename: crates-io-index-api-openapi.yml
  format: yaml
  label: crates.io Index API
  slug: crates-io-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/openapi/crates-io-index-api-openapi.yml
- filename: crates-io-owners-api-openapi.yml
  format: yaml
  label: crates.io Owners API
  slug: crates-io-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/openapi/crates-io-owners-api-openapi.yml
- filename: crates-io-versions-api-openapi.yml
  format: yaml
  label: crates.io Versions API
  slug: crates-io-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/openapi/crates-io-versions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Crates Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: crates.io secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: crates.io
provider_slug: crates-io
scheme_count: 1
schemes:
- description: A crates.io API token created at https://crates.io/settings/tokens. The raw token is sent in the Authorization header without a Bearer prefix.
  in: header
  name: ApiTokenAuth
  parameter: Authorization
  sources:
  - openapi/crates-io-web-api-openapi.yml
  type: apiKey
slug: crates-io-authentication
source_filename: crates-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/crates-io-web-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiTokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: A crates.io API token created at https://crates.io/settings/tokens. The raw token\n    is sent in the Authorization header without a Bearer prefix.\n  sources:\n  - openapi/crates-io-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/authentication/crates-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Rust
- Package Registry
- Crates
- Cargo
- Open-Source
- Developer Tools
- Rust Foundation
---
