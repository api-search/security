---
anonymous_access: false
api_key_in: []
api_specs:
- filename: checkout-checkout-api-api-openapi.yml
  format: yaml
  label: Checkout Checkout API
  slug: checkout-checkout-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkout/refs/heads/main/openapi/checkout-checkout-api-api-openapi.yml
- filename: checkout-connect-api-openapi.yml
  format: yaml
  label: Checkout Connect API
  slug: checkout-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkout/refs/heads/main/openapi/checkout-connect-api-openapi.yml
- filename: checkout-payments-api-openapi.yml
  format: yaml
  label: Checkout Payments API
  slug: checkout-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkout/refs/heads/main/openapi/checkout-payments-api-openapi.yml
auth_types: []
description: Authentication schemes for Checkout.com API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Checkout Authentication
name_suffix: Authentication
oauth_flows: []
overview: Checkout declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Checkout
provider_slug: checkout
scheme_count: 1
schemes:
- evidence: To use an API key in your API request, provide it in the Authorization header with the Bearer Prefix.
  header: Authorization
  how_to_obtain: Generate public and secret API keys in the Checkout.com Dashboard.
  location: header
  name: API Key
  type: http-bearer
slug: checkout-authentication
source_filename: checkout-authentication.yml
source_heading: Authentication Profile
source_url: https://www.checkout.com/products/authentication-3ds
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.checkout.com/products/authentication-3ds\nsources:\n- https://www.checkout.com/products/authentication-3ds\n- https://www.checkout.com/resources/authentication\n- https://www.checkout.com/docs/developer-resources/api/manage-api-keys/api-keys\n- https://www.checkout.com/docs/business-operations/ensure-regulatory-compliance\ndescription: Authentication schemes for Checkout.com API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: To use an API key in your API request, provide it in the Authorization header with the Bearer Prefix.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate public and secret API keys in the Checkout.com Dashboard.\nnote: No OAuth2 or other authentication schemes are documented on the provided pages.\ndocs: https://www.checkout.com/products/authentication-3ds\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkout/refs/heads/main/authentication/checkout-authentication.yml
summary_line: 1 scheme
tags:
- Payments
- Fintech
- E-Commerce
- Global
---
