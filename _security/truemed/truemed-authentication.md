---
anonymous_access: false
api_key_in: []
api_specs:
- filename: truemed-disputes-api-openapi.yml
  format: yaml
  label: Truemed Disputes API
  slug: truemed-disputes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-disputes-api-openapi.yml
- filename: truemed-eligibility-api-openapi.yml
  format: yaml
  label: Truemed Eligibility API
  slug: truemed-eligibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-eligibility-api-openapi.yml
- filename: truemed-files-api-openapi.yml
  format: yaml
  label: Truemed Files API
  slug: truemed-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-files-api-openapi.yml
- filename: truemed-paymentsessions-api-openapi.yml
  format: yaml
  label: Truemed Payment Sessions API
  slug: truemed-paymentsessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-paymentsessions-api-openapi.yml
- filename: truemed-paymenttokens-api-openapi.yml
  format: yaml
  label: Truemed Payment Tokens API
  slug: truemed-paymenttokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-paymenttokens-api-openapi.yml
- filename: truemed-qualificationsessions-api-openapi.yml
  format: yaml
  label: Truemed Qualification Sessions API
  slug: truemed-qualificationsessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-qualificationsessions-api-openapi.yml
- filename: truemed-reconciliations-api-openapi.yml
  format: yaml
  label: Truemed Reconciliations API
  slug: truemed-reconciliations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-reconciliations-api-openapi.yml
- filename: truemed-product-catalog-api-openapi.yml
  format: yaml
  label: Truemed Product Catalog API
  slug: truemed-product-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-product-catalog-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Truemed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Truemed declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Truemed
provider_slug: truemed
scheme_count: 1
schemes:
- evidence: Authentication x-truemed-api-key string Sales channel API key for merchant server-to-server authentication
  header: x-truemed-api-key
  location: header
  name: x-truemed-api-key
  type: apiKey
slug: truemed-authentication
source_filename: truemed-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.truemed.com/guides/setup/api/subscriptions/token-lifecycle
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.truemed.com/guides/setup/api/subscriptions/token-lifecycle\nsources:\n- https://developers.truemed.com/guides/setup/api/subscriptions/token-lifecycle\n- https://developers.truemed.com/api-reference/payment-tokens/create-payment-token\n- https://developers.truemed.com/api-reference/payment-tokens/retrieve-payment-token\n- https://developers.truemed.com/api-reference/payment-tokens/list-payment-token\nschemes:\n- type: apiKey\n  name: x-truemed-api-key\n  evidence: Authentication x-truemed-api-key string Sales channel API key for merchant server-to-server authentication\n  location: header\n  header: x-truemed-api-key\ndocs: https://developers.truemed.com/guides/setup/api/subscriptions/token-lifecycle\n"
source_yaml_url: https://artifacts.apis.io/truemed/authentication/truemed-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Health
- Fintech
- HSA
- FSA
- Payments
---
