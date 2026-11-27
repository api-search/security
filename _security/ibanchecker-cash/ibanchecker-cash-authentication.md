---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ibanchecker-cash-extract-api-openapi.yml
  format: yaml
  label: IBAN Checker Extract API
  slug: ibanchecker-cash-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ibanchecker-cash/openapi/ibanchecker-cash-extract-api-openapi.yml
- filename: ibanchecker-cash-formats-api-openapi.yml
  format: yaml
  label: IBAN Checker Formats API
  slug: ibanchecker-cash-formats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ibanchecker-cash/openapi/ibanchecker-cash-formats-api-openapi.yml
- filename: ibanchecker-cash-swift-api-openapi.yml
  format: yaml
  label: IBAN Checker Swift API
  slug: ibanchecker-cash-swift-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ibanchecker-cash/openapi/ibanchecker-cash-swift-api-openapi.yml
- filename: ibanchecker-cash-validate-api-openapi.yml
  format: yaml
  label: IBAN Checker Validate API
  slug: ibanchecker-cash-validate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ibanchecker-cash/openapi/ibanchecker-cash-validate-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: IBAN Checker Authentication
name_suffix: Authentication
oauth_flows: []
overview: IBAN Checker secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IBAN Checker
provider_slug: ibanchecker-cash
scheme_count: 1
schemes:
- description: API key issued at https://ibanchecker.cash/api-docs; the free key covers 100 requests a month of single validation. Required for every endpoint except /formats. Bulk validation and BIC lookup need the Basic plan, extraction the Growth plan; a free key whose address has a verified ibanchecker.cash account can try them (up to 10 IBANs per bulk call, 5,000 characters per extraction). Bulk and extract
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ibanchecker-cash-openapi.json
  type: http
slug: ibanchecker-cash-authentication
source_filename: ibanchecker-cash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/ibanchecker-cash-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key issued at https://ibanchecker.cash/api-docs; the free key covers 100\n    requests a month of single validation. Required for every endpoint except /formats. Bulk\n    validation and BIC lookup need the Basic plan, extraction the Growth plan; a free key whose\n    address has a verified ibanchecker.cash account can try them (up to 10 IBANs per bulk call,\n    5,000 characters per extraction). Bulk and extract\n  sources:\n  - openapi/ibanchecker-cash-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/ibanchecker-cash/authentication/ibanchecker-cash-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Finance
- Banking
- Validation
---
