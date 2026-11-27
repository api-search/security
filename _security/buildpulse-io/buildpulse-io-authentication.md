---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: buildpulse-io-auth-api-openapi.yml
  format: yaml
  label: BuildPulse Auth API
  slug: buildpulse-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-auth-api-openapi.yml
- filename: buildpulse-io-badges-api-openapi.yml
  format: yaml
  label: BuildPulse Badges API
  slug: buildpulse-io-badges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-badges-api-openapi.yml
- filename: buildpulse-io-flaky-api-openapi.yml
  format: yaml
  label: BuildPulse Flaky API
  slug: buildpulse-io-flaky-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-flaky-api-openapi.yml
- filename: buildpulse-io-health-api-openapi.yml
  format: yaml
  label: BuildPulse Health API
  slug: buildpulse-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-health-api-openapi.yml
- filename: buildpulse-io-submissions-api-openapi.yml
  format: yaml
  label: BuildPulse Submissions API
  slug: buildpulse-io-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-submissions-api-openapi.yml
- filename: buildpulse-io-tests-api-openapi.yml
  format: yaml
  label: BuildPulse Tests API
  slug: buildpulse-io-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-tests-api-openapi.yml
- filename: buildpulse-io-webhooks-api-openapi.yml
  format: yaml
  label: BuildPulse Webhooks API
  slug: buildpulse-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: BuildPulse Authentication
name_suffix: Authentication
oauth_flows: []
overview: BuildPulse secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BuildPulse
provider_slug: buildpulse-io
scheme_count: 2
schemes:
- description: "Send `Authorization: token <token>`. Two token shapes are\naccepted:\n\n- **New** (`bp_<64-hex>`) — minted by the refactored web-client\n  today (`web-client/src/app/_services/apiTokens.ts`). Stored as\n  `{ type: \"api_token\", tokenPrefix, tokenHash (hex SHA256),\n  expiresAt }`. No active-plan gate; issuance is the\n  entitlement check.\n- **Legacy** (`<40-hex>`) — Rails-era format, stored as\n  `{ hashed"
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/buildpulse-io-openapi.yaml
  type: apiKey
- bearerFormat: bp_<64-hex> or <40-hex>
  description: 'Send `Authorization: Bearer <token>`. Functionally identical to

    `TokenAuth`; both header forms are accepted. Same two token

    shapes apply — see `TokenAuth` for the format and plan-gate

    details.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/buildpulse-io-openapi.yaml
  type: http
slug: buildpulse-io-authentication
source_filename: buildpulse-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/buildpulse-io-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Send `Authorization: token <token>`. Two token shapes are\n    accepted:\n\n    - **New** (`bp_<64-hex>`) — minted by the refactored web-client\n      today (`web-client/src/app/_services/apiTokens.ts`). Stored as\n      `{ type: \"api_token\", tokenPrefix, tokenHash (hex SHA256),\n      expiresAt }`. No active-plan gate; issuance is the\n      entitlement check.\n    - **Legacy** (`<40-hex>`) — Rails-era format, stored as\n      `{ hashed\n  sources:\n  - openapi/buildpulse-io-openapi.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: bp_<64-hex> or <40-hex>\n  description: |-\n    Send `Authorization: Bearer <token>`. Functionally identical to\n    `TokenAuth`; both header forms are accepted.\
  \ Same two token\n    shapes apply — see `TokenAuth` for the format and plan-gate\n    details.\n  sources:\n  - openapi/buildpulse-io-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/buildpulse-io/authentication/buildpulse-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- CI
- DevOps
- Testing
- Artificial Intelligence
- Analytics
- Company
---
