---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gembook-xyz-assets-api-openapi.yml
  format: yaml
  label: Gembook Assets API
  slug: gembook-xyz-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gembook-xyz/openapi/gembook-xyz-assets-api-openapi.yml
- filename: gembook-xyz-market-api-openapi.yml
  format: yaml
  label: Gembook Market API
  slug: gembook-xyz-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gembook-xyz/openapi/gembook-xyz-market-api-openapi.yml
- filename: gembook-xyz-meta-api-openapi.yml
  format: yaml
  label: Gembook Meta API
  slug: gembook-xyz-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gembook-xyz/openapi/gembook-xyz-meta-api-openapi.yml
- filename: gembook-xyz-sets-api-openapi.yml
  format: yaml
  label: Gembook Sets API
  slug: gembook-xyz-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gembook-xyz/openapi/gembook-xyz-sets-api-openapi.yml
- filename: gembook-xyz-webhooks-api-openapi.yml
  format: yaml
  label: Gembook Webhooks API
  slug: gembook-xyz-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gembook-xyz/openapi/gembook-xyz-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Gembook Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gembook secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gembook
provider_slug: gembook-xyz
scheme_count: 1
schemes:
- description: 'API key issued via the operator CLI. Format: gemb_<48 char base64url>'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/gembook-xyz-openapi.json
  type: http
slug: gembook-xyz-authentication
source_filename: gembook-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/gembook-xyz-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: 'API key issued via the operator CLI. Format: gemb_<48 char base64url>'\n  sources:\n  - openapi/gembook-xyz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/gembook-xyz/authentication/gembook-xyz-authentication.yml
summary_line: http · 1 scheme
tags:
- Pokemon
- Pricing
- Collectibles
- PSA
---
