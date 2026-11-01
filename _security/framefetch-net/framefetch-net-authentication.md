---
anonymous_access: false
api_key_in: []
api_specs:
- filename: framefetch-net-account-api-openapi.yml
  format: yaml
  label: framefetch-net Account API
  slug: framefetch-net-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-account-api-openapi.yml
- filename: framefetch-net-batch-api-openapi.yml
  format: yaml
  label: framefetch-net Batch API
  slug: framefetch-net-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-batch-api-openapi.yml
- filename: framefetch-net-billing-api-openapi.yml
  format: yaml
  label: framefetch-net Billing API
  slug: framefetch-net-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-billing-api-openapi.yml
- filename: framefetch-net-checkout-api-openapi.yml
  format: yaml
  label: framefetch-net Checkout API
  slug: framefetch-net-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-checkout-api-openapi.yml
- filename: framefetch-net-demo-api-openapi.yml
  format: yaml
  label: framefetch-net Demo API
  slug: framefetch-net-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-demo-api-openapi.yml
- filename: framefetch-net-extract-api-openapi.yml
  format: yaml
  label: framefetch-net Extract API
  slug: framefetch-net-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-extract-api-openapi.yml
- filename: framefetch-net-framefetch-api-api-openapi.yml
  format: yaml
  label: framefetch-net FrameFetch API
  slug: framefetch-net-framefetch-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-framefetch-api-api-openapi.yml
- filename: framefetch-net-frames-api-openapi.yml
  format: yaml
  label: framefetch-net Frames API
  slug: framefetch-net-frames-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-frames-api-openapi.yml
- filename: framefetch-net-healthz-api-openapi.yml
  format: yaml
  label: framefetch-net Healthz API
  slug: framefetch-net-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-healthz-api-openapi.yml
- filename: framefetch-net-keys-api-openapi.yml
  format: yaml
  label: framefetch-net Keys API
  slug: framefetch-net-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-keys-api-openapi.yml
- filename: framefetch-net-metadata-api-openapi.yml
  format: yaml
  label: framefetch-net Metadata API
  slug: framefetch-net-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-metadata-api-openapi.yml
- filename: framefetch-net-platforms-api-openapi.yml
  format: yaml
  label: framefetch-net Platforms API
  slug: framefetch-net-platforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-platforms-api-openapi.yml
- filename: framefetch-net-status-api-openapi.yml
  format: yaml
  label: framefetch-net Status API
  slug: framefetch-net-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-status-api-openapi.yml
- filename: framefetch-net-transcript-api-openapi.yml
  format: yaml
  label: framefetch-net Transcript API
  slug: framefetch-net-transcript-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-transcript-api-openapi.yml
- filename: framefetch-net-usage-api-openapi.yml
  format: yaml
  label: framefetch-net Usage API
  slug: framefetch-net-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-usage-api-openapi.yml
- filename: framefetch-net-watch-api-openapi.yml
  format: yaml
  label: framefetch-net Watch API
  slug: framefetch-net-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-watch-api-openapi.yml
- filename: framefetch-net-top-up-api-openapi.yml
  format: yaml
  label: framefetch-net Top Up API
  slug: framefetch-net-top-up-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-top-up-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Framefetch Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: framefetch-net secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: framefetch-net
provider_slug: framefetch-net
scheme_count: 1
schemes:
- description: 'API key from POST /v1/keys, sent as ''Authorization: Bearer <key>''.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/framefetch-net-openapi.json
  type: http
slug: framefetch-net-authentication
source_filename: framefetch-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/framefetch-net-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key from POST /v1/keys, sent as ''Authorization: Bearer <key>''.'\n  sources:\n  - openapi/framefetch-net-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/framefetch-net/authentication/framefetch-net-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Video
- AI
- DataAPI
- Media
---
