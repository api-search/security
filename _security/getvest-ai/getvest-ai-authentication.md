---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getvest-ai-claim-api-openapi.yml
  format: yaml
  label: Vest Claim API
  slug: getvest-ai-claim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvest-ai/openapi/getvest-ai-claim-api-openapi.yml
- filename: getvest-ai-estimate-api-openapi.yml
  format: yaml
  label: Vest Estimate API
  slug: getvest-ai-estimate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvest-ai/openapi/getvest-ai-estimate-api-openapi.yml
- filename: getvest-ai-stack-api-openapi.yml
  format: yaml
  label: Vest Stack API
  slug: getvest-ai-stack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvest-ai/openapi/getvest-ai-stack-api-openapi.yml
- filename: getvest-ai-submit-tool-api-openapi.yml
  format: yaml
  label: Vest Submit Tool API
  slug: getvest-ai-submit-tool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvest-ai/openapi/getvest-ai-submit-tool-api-openapi.yml
- filename: getvest-ai-tools-api-openapi.yml
  format: yaml
  label: Vest Tools API
  slug: getvest-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvest-ai/openapi/getvest-ai-tools-api-openapi.yml
- filename: getvest-ai-wallet-api-openapi.yml
  format: yaml
  label: Vest Wallet API
  slug: getvest-ai-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvest-ai/openapi/getvest-ai-wallet-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Vest Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vest secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vest
provider_slug: getvest-ai
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/getvest-ai-openapi.json
  type: http
slug: getvest-ai-authentication
source_filename: getvest-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/getvest-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/getvest-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getvest-ai/authentication/getvest-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Partnerships
- Growth Platform
- Channel Management
- Marketplace Integration
---
