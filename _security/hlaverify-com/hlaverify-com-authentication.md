---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: hlaverify-com-admin-api-openapi.yml
  format: yaml
  label: HLA-Verify Admin API
  slug: hlaverify-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-admin-api-openapi.yml
- filename: hlaverify-com-allele-api-openapi.yml
  format: yaml
  label: HLA-Verify Allele API
  slug: hlaverify-com-allele-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-allele-api-openapi.yml
- filename: hlaverify-com-beta-signup-api-openapi.yml
  format: yaml
  label: HLA-Verify Beta Signup API
  slug: hlaverify-com-beta-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-beta-signup-api-openapi.yml
- filename: hlaverify-com-checkout-api-openapi.yml
  format: yaml
  label: HLA-Verify Checkout API
  slug: hlaverify-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-checkout-api-openapi.yml
- filename: hlaverify-com-compat-api-openapi.yml
  format: yaml
  label: HLA-Verify Compat API
  slug: hlaverify-com-compat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-compat-api-openapi.yml
- filename: hlaverify-com-glstring-api-openapi.yml
  format: yaml
  label: HLA-Verify Glstring API
  slug: hlaverify-com-glstring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-glstring-api-openapi.yml
- filename: hlaverify-com-healthz-api-openapi.yml
  format: yaml
  label: HLA-Verify Healthz API
  slug: hlaverify-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-healthz-api-openapi.yml
- filename: hlaverify-com-keys-api-openapi.yml
  format: yaml
  label: HLA-Verify Keys API
  slug: hlaverify-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-keys-api-openapi.yml
- filename: hlaverify-com-match-api-openapi.yml
  format: yaml
  label: HLA-Verify Match API
  slug: hlaverify-com-match-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-match-api-openapi.yml
- filename: hlaverify-com-mcp-api-openapi.yml
  format: yaml
  label: HLA-Verify MCP API
  slug: hlaverify-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-mcp-api-openapi.yml
- filename: hlaverify-com-normalize-api-openapi.yml
  format: yaml
  label: HLA-Verify Normalize API
  slug: hlaverify-com-normalize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-normalize-api-openapi.yml
- filename: hlaverify-com-pgx-api-openapi.yml
  format: yaml
  label: HLA-Verify Pgx API
  slug: hlaverify-com-pgx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-pgx-api-openapi.yml
- filename: hlaverify-com-pricing-api-openapi.yml
  format: yaml
  label: HLA-Verify Pricing API
  slug: hlaverify-com-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-pricing-api-openapi.yml
- filename: hlaverify-com-releases-api-openapi.yml
  format: yaml
  label: HLA-Verify Releases API
  slug: hlaverify-com-releases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-releases-api-openapi.yml
- filename: hlaverify-com-report-api-openapi.yml
  format: yaml
  label: HLA-Verify Report API
  slug: hlaverify-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-report-api-openapi.yml
- filename: hlaverify-com-research-access-api-openapi.yml
  format: yaml
  label: HLA-Verify Research Access API
  slug: hlaverify-com-research-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-research-access-api-openapi.yml
- filename: hlaverify-com-translate-api-openapi.yml
  format: yaml
  label: HLA-Verify Translate API
  slug: hlaverify-com-translate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-translate-api-openapi.yml
- filename: hlaverify-com-typing-api-openapi.yml
  format: yaml
  label: HLA-Verify Typing API
  slug: hlaverify-com-typing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-typing-api-openapi.yml
- filename: hlaverify-com-usage-api-openapi.yml
  format: yaml
  label: HLA-Verify Usage API
  slug: hlaverify-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-usage-api-openapi.yml
- filename: hlaverify-com-verify-api-openapi.yml
  format: yaml
  label: HLA-Verify Verify API
  slug: hlaverify-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hlaverify-com/openapi/hlaverify-com-verify-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: HLA-Verify Authentication
name_suffix: Authentication
oauth_flows: []
overview: HLA-Verify secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HLA-Verify
provider_slug: hlaverify-com
scheme_count: 1
schemes:
- in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/hlaverify-com-openapi.json
  type: apiKey
slug: hlaverify-com-authentication
source_filename: hlaverify-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hlaverify-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/hlaverify-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hlaverify-com/authentication/hlaverify-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Bioinformatics
- Healthcare
- Verification
---
