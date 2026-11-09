---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bitrefill-account-api-openapi.yml
  format: yaml
  label: Bitrefill Account API
  slug: bitrefill-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitrefill/openapi/bitrefill-account-api-openapi.yml
- filename: bitrefill-checkout-api-openapi.yml
  format: yaml
  label: Bitrefill Checkout API
  slug: bitrefill-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitrefill/openapi/bitrefill-checkout-api-openapi.yml
- filename: bitrefill-discovery-api-openapi.yml
  format: yaml
  label: Bitrefill Discovery API
  slug: bitrefill-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitrefill/openapi/bitrefill-discovery-api-openapi.yml
- filename: bitrefill-payments-api-openapi.yml
  format: yaml
  label: Bitrefill Payments API
  slug: bitrefill-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitrefill/openapi/bitrefill-payments-api-openapi.yml
auth_types: []
description: Authentication methods for Bitrefill API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bitrefill Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitrefill declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bitrefill
provider_slug: bitrefill
scheme_count: 2
schemes:
- evidence: 'const headers = { ''Authorization'': `Bearer ${API_KEY}`, ''Content-Type'': ''application/json'' };'
  header: Authorization
  how_to_obtain: Generate an API key in the Bitrefill account developers page.
  location: header
  name: Bearer
  type: http-bearer
- evidence: All supported clients work with OAuth — just add the server URL and sign in when prompted.
  how_to_obtain: Use the OAuth flow provided by the MCP server (e.g., via client UI).
  name: OAuth
  type: oauth2
slug: bitrefill-authentication
source_filename: bitrefill-authentication.yml
source_heading: Authentication Profile
source_url: https://help.bitrefill.com/hc/en-us/articles/4402564626450-How-to-add-store-credit-by-paying-with-tokens-from-my-wallet
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.bitrefill.com/hc/en-us/articles/4402564626450-How-to-add-store-credit-by-paying-with-tokens-from-my-wallet\nsources:\n- https://help.bitrefill.com/hc/en-us/articles/4402564626450-How-to-add-store-credit-by-paying-with-tokens-from-my-wallet\n- https://help.bitrefill.com/hc/en-us/articles/11000339909266-Can-I-purchase-gift-cards-using-my-favorite-token\n- https://docs.bitrefill.com/docs/quickstart-2.md\n- https://docs.bitrefill.com/docs/setup-guides.md\ndescription: Authentication methods for Bitrefill API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'const headers = { ''Authorization'': `Bearer ${API_KEY}`, ''Content-Type'': ''application/json'' };'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the Bitrefill account developers page.\n- type: oauth2\n  name: OAuth\n  evidence: All supported clients work with OAuth\
  \ — just add the server URL and sign in when prompted.\n  how_to_obtain: Use the OAuth flow provided by the MCP server (e.g., via client UI).\ndocs: https://help.bitrefill.com/hc/en-us/articles/4402564626450-How-to-add-store-credit-by-paying-with-tokens-from-my-wallet\n"
source_yaml_url: https://artifacts.apis.io/bitrefill/authentication/bitrefill-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cryptocurrency
- Payments
- Gift Cards
- Mobile Top-Up
---
