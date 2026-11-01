---
anonymous_access: false
api_key_in: []
api_specs:
- filename: grainfinance-co-conversions-api-openapi.yml
  format: yaml
  label: Grain Conversions API
  slug: grainfinance-co-conversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-conversions-api-openapi.yml
- filename: grainfinance-co-customers-api-openapi.yml
  format: yaml
  label: Grain Customers API
  slug: grainfinance-co-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-customers-api-openapi.yml
- filename: grainfinance-co-dual-hedges-api-openapi.yml
  format: yaml
  label: Grain Dual Hedges API
  slug: grainfinance-co-dual-hedges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-dual-hedges-api-openapi.yml
- filename: grainfinance-co-grain-api-api-openapi.yml
  format: yaml
  label: Grain Grain API
  slug: grainfinance-co-grain-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-grain-api-api-openapi.yml
- filename: grainfinance-co-hedges-api-openapi.yml
  format: yaml
  label: Grain Hedges API
  slug: grainfinance-co-hedges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-hedges-api-openapi.yml
- filename: grainfinance-co-payouts-api-openapi.yml
  format: yaml
  label: Grain Payouts API
  slug: grainfinance-co-payouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-payouts-api-openapi.yml
- filename: grainfinance-co-pricing-api-openapi.yml
  format: yaml
  label: Grain Pricing API
  slug: grainfinance-co-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-pricing-api-openapi.yml
- filename: grainfinance-co-vendors-api-openapi.yml
  format: yaml
  label: Grain Vendors API
  slug: grainfinance-co-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-vendors-api-openapi.yml
- filename: grainfinance-co-wallets-api-openapi.yml
  format: yaml
  label: Grain Wallets API
  slug: grainfinance-co-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-wallets-api-openapi.yml
auth_types: []
description: Authentication schemes for Grain API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Grainfinance Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Grain declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Grain
provider_slug: grainfinance-co
scheme_count: 1
schemes:
- evidence: All endpoints use **HTTP Basic Authentication**. Your Client ID is the username and your Secret is the password.
  header: Authorization
  how_to_obtain: Find your credentials in the Grain Dashboard under Developer → API Keys (separate for Sandbox and Live environments).
  location: header
  name: HTTP Basic
  type: http-basic
slug: grainfinance-co-authentication
source_filename: grainfinance-co-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.grainfinance.co/get-started/retrieve-api-keys.md
source_yaml: "generated: '2026-10-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.grainfinance.co/get-started/retrieve-api-keys.md\nsources:\n- https://docs.grainfinance.co/get-started/retrieve-api-keys.md\n- https://docs.grainfinance.co/api-reference/authentication.md\n- https://docs.grainfinance.co/get-started/setup-your-configuration.md\n- https://docs.grainfinance.co/webhooks/index.md\ndescription: Authentication schemes for Grain API\nschemes:\n- type: http-basic\n  name: HTTP Basic\n  evidence: All endpoints use **HTTP Basic Authentication**. Your Client ID is the username and your Secret is the password.\n  location: header\n  header: Authorization\n  how_to_obtain: Find your credentials in the Grain Dashboard under Developer → API Keys (separate for Sandbox and Live environments).\ndocs: https://docs.grainfinance.co/get-started/retrieve-api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/grainfinance-co/authentication/grainfinance-co-authentication.yml
summary_line: 1 scheme
tags:
- Fintech
- Payments
- Currency
- API
- Embedded
---
