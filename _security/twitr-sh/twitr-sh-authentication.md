---
anonymous_access: false
api_key_in: []
api_specs:
- filename: twitr-sh-accounts-api-openapi.yml
  format: yaml
  label: twitr-sh Accounts API
  slug: twitr-sh-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-accounts-api-openapi.yml
- filename: twitr-sh-creator-api-openapi.yml
  format: yaml
  label: twitr-sh Creator API
  slug: twitr-sh-creator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-creator-api-openapi.yml
- filename: twitr-sh-intelligence-api-openapi.yml
  format: yaml
  label: twitr-sh Intelligence API
  slug: twitr-sh-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-intelligence-api-openapi.yml
- filename: twitr-sh-monitors-api-openapi.yml
  format: yaml
  label: twitr-sh Monitors API
  slug: twitr-sh-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-monitors-api-openapi.yml
- filename: twitr-sh-search-api-openapi.yml
  format: yaml
  label: twitr-sh Search API
  slug: twitr-sh-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-search-api-openapi.yml
- filename: twitr-sh-snapshots-api-openapi.yml
  format: yaml
  label: twitr-sh Snapshots API
  slug: twitr-sh-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-snapshots-api-openapi.yml
- filename: twitr-sh-social-api-openapi.yml
  format: yaml
  label: twitr-sh Social API
  slug: twitr-sh-social-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-social-api-openapi.yml
- filename: twitr-sh-webhooks-api-openapi.yml
  format: yaml
  label: twitr-sh Webhooks API
  slug: twitr-sh-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Twitr Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: twitr-sh declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: twitr-sh
provider_slug: twitr-sh
scheme_count: 3
schemes:
- description: API key for SIWX payments
  in: header
  name: siwx
  official: true
  type: apiKey
- bearerFormat: JWT
  description: Bearer token for optional API key usage
  name: bearerKey
  official: true
  scheme: bearer
  type: http
- description: Public read access API key
  in: header
  name: publicRead
  official: true
  type: apiKey
slug: twitr-sh-authentication
source_filename: twitr-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://twitr.sh/openapi.json\nschemes:\n  - name: siwx\n    type: apiKey\n    in: header\n    description: API key for SIWX payments\n    official: true\n  - name: bearerKey\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token for optional API key usage\n    official: true\n  - name: publicRead\n    type: apiKey\n    in: header\n    description: Public read access API key\n    official: true\n"
source_yaml_url: https://artifacts.apis.io/twitr-sh/authentication/twitr-sh-authentication.yml
summary_line: 3 schemes
tags:
- Company
- API
- X
- Twitter
- Pay-per-call
- AI
---
