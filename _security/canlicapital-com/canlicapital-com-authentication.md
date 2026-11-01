---
anonymous_access: false
api_key_in: []
api_specs:
- filename: canlicapital-com-chain-api-openapi.yml
  format: yaml
  label: canlicapital-com Chain API
  slug: canlicapital-com-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-chain-api-openapi.yml
- filename: canlicapital-com-keys-api-openapi.yml
  format: yaml
  label: canlicapital-com Keys API
  slug: canlicapital-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-keys-api-openapi.yml
- filename: canlicapital-com-receipts-api-openapi.yml
  format: yaml
  label: canlicapital-com Receipts API
  slug: canlicapital-com-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-receipts-api-openapi.yml
- filename: canlicapital-com-record-api-openapi.yml
  format: yaml
  label: canlicapital-com Record API
  slug: canlicapital-com-record-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-record-api-openapi.yml
- filename: canlicapital-com-research-api-openapi.yml
  format: yaml
  label: canlicapital-com Research API
  slug: canlicapital-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-research-api-openapi.yml
- filename: canlicapital-com-sleeves-api-openapi.yml
  format: yaml
  label: canlicapital-com Sleeves API
  slug: canlicapital-com-sleeves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-sleeves-api-openapi.yml
- filename: canlicapital-com-status-api-openapi.yml
  format: yaml
  label: canlicapital-com Status API
  slug: canlicapital-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-status-api-openapi.yml
- filename: canlicapital-com-trials-api-openapi.yml
  format: yaml
  label: canlicapital-com Trials API
  slug: canlicapital-com-trials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-trials-api-openapi.yml
- filename: canlicapital-com-validate-api-openapi.yml
  format: yaml
  label: canlicapital-com Validate API
  slug: canlicapital-com-validate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-validate-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Canlicapital Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: canlicapital-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: canlicapital-com
provider_slug: canlicapital-com
scheme_count: 1
schemes:
- description: 'A key from POST /api/v1/keys, sent as Authorization: Bearer ck_live_...'
  name: bearerKey
  scheme: bearer
  sources:
  - openapi/canlicapital-com-openapi-site.json
  - openapi/canlicapital-com-openapi.json
  type: http
slug: canlicapital-com-authentication
source_filename: canlicapital-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/canlicapital-com-openapi-site.json, openapi/canlicapital-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerKey\n  type: http\n  scheme: bearer\n  description: 'A key from POST /api/v1/keys, sent as Authorization: Bearer ck_live_...'\n  sources:\n  - openapi/canlicapital-com-openapi-site.json\n  - openapi/canlicapital-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/canlicapital-com/authentication/canlicapital-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Data
- AI
- QuantitativeTools
- DeveloperAPI
---
