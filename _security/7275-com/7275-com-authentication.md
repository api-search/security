---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 7275-com-activity-api-openapi.yml
  format: yaml
  label: DEXUN Inc Activity API
  slug: 7275-com-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/7275-com/openapi/7275-com-activity-api-openapi.yml
- filename: 7275-com-identity-api-openapi.yml
  format: yaml
  label: DEXUN Inc Identity API
  slug: 7275-com-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/7275-com/openapi/7275-com-identity-api-openapi.yml
- filename: 7275-com-keys-api-openapi.yml
  format: yaml
  label: DEXUN Inc Keys API
  slug: 7275-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/7275-com/openapi/7275-com-keys-api-openapi.yml
- filename: 7275-com-public-api-openapi.yml
  format: yaml
  label: DEXUN Inc Public API
  slug: 7275-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/7275-com/openapi/7275-com-public-api-openapi.yml
- filename: 7275-com-quota-api-openapi.yml
  format: yaml
  label: DEXUN Inc Quota API
  slug: 7275-com-quota-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/7275-com/openapi/7275-com-quota-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: 7275 Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DEXUN Inc secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DEXUN Inc
provider_slug: 7275-com
scheme_count: 1
schemes:
- bearerFormat: dxk_<env>_<token>
  description: Generate in /settings/api-keys. Plaintext is shown once at creation; only the SHA-256 hash is stored.
  name: BearerApiKey
  scheme: bearer
  sources:
  - openapi/7275-com-openapi.json
  type: http
slug: 7275-com-authentication
source_filename: 7275-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/7275-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: dxk_<env>_<token>\n  description: Generate in /settings/api-keys. Plaintext is shown once at creation; only the\n    SHA-256 hash is stored.\n  sources:\n  - openapi/7275-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/7275-com/authentication/7275-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Advertising
- Artificial Intelligence
- Marketing
- Multi-Account
- Automation
---
