---
anonymous_access: false
api_key_in: []
api_specs:
- filename: two-api-key-api-openapi.yml
  format: yaml
  label: Two API Key API
  slug: two-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-api-key-api-openapi.yml
- filename: two-invoice-api-openapi.yml
  format: yaml
  label: Two Invoice API
  slug: two-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-invoice-api-openapi.yml
- filename: two-order-api-openapi.yml
  format: yaml
  label: Two Order API
  slug: two-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-order-api-openapi.yml
- filename: two-order-intent-api-openapi.yml
  format: yaml
  label: Two Order intent API
  slug: two-order-intent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-order-intent-api-openapi.yml
- filename: two-settlement-report-api-openapi.yml
  format: yaml
  label: Two Settlement report API
  slug: two-settlement-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-settlement-report-api-openapi.yml
auth_types: []
description: Two uses API keys passed in the X-Api-Key header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Two Authentication
name_suffix: Authentication
oauth_flows: []
overview: Two declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Two
provider_slug: two
scheme_count: 1
schemes:
- evidence: '**Authentication:** X-Api-Key'
  header: X-Api-Key
  how_to_obtain: API keys are generated in the Merchant Portal integration panel (see the Getting API Keys guide).
  location: header
  name: X-Api-Key
  type: apiKey
slug: two-authentication
source_filename: two-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.two.inc/llms/guides/getting-api-keys-page.txt
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.two.inc/llms/guides/getting-api-keys-page.txt\nsources:\n- https://docs.two.inc/llms/guides/getting-api-keys-page.txt\n- https://docs.two.inc/llms/api/checkout/retrieve-merchant-api-keys-handler-get.txt\n- https://docs.two.inc/llms/api/checkout/create-merchant-api-key-handler-post.txt\n- https://docs.two.inc/llms/api/checkout/retrieve-merchant-api-key-handler-get.txt\ndescription: Two uses API keys passed in the X-Api-Key header.\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: '**Authentication:** X-Api-Key'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: API keys are generated in the Merchant Portal integration panel (see the Getting API Keys guide).\ndocs: https://docs.two.inc/llms/guides/getting-api-keys-page.txt\n"
source_yaml_url: https://artifacts.apis.io/two/authentication/two-authentication.yml
summary_line: 1 scheme
tags:
- Company
- B2B Payments
- FinTech
- API Platform
- Checkout
- Trade Accounts
---
