---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ccbill-openapi-generated.yml
  format: yaml
  label: Ccbill API
  slug: ccbill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ccbill/openapi/_ae-authored/ccbill-openapi-generated.yml
auth_types: []
description: CCBill uses OAuth 2.0 client‑credentials flow. Front‑end credentials (Merchant Application ID and Secret Key) are Base64‑encoded and sent with HTTP Basic authentication to obtain an access token, which is then sent as a Bearer token in the Authorization header of API calls.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ccbill Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ccbill declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ccbill
provider_slug: ccbill
scheme_count: 2
schemes:
- evidence: The CCBill RESTful API uses OAuth-based authentication and authorization. Use the frontend credentials ( Merchant Application ID and Secret Key that are Base64 encoded) you received from Merchant Support to generate a frontend bearer token .
  header: Authorization
  how_to_obtain: Provide the Frontend_Merchant_Application_ID and Frontend_Secret_Key as the username and password (‑u) in a POST to the token endpoint with grant_type=client_credentials.
  location: header
  name: Basic
  token_url: https://api.ccbill.com/ccbill-auth/oauth/token
  type: http-basic
- evidence: You must include this token in the Authorization header of API requests when creating payment tokens.
  header: Authorization
  how_to_obtain: Use the access token returned from the client_credentials token request as a Bearer token.
  location: header
  name: Bearer
  token_url: https://api.ccbill.com/ccbill-auth/oauth/token
  type: http-bearer
slug: ccbill-authentication
source_filename: ccbill-authentication.yml
source_heading: Authentication Profile
source_url: https://ccbill.com/doc/create-payment-token-non-3ds
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ccbill.com/doc/create-payment-token-non-3ds\nsources:\n- https://ccbill.com/doc/create-payment-token-non-3ds\n- https://ccbill.com/doc/create-payment-token-3ds\n- https://ccbill.com/doc/create-payment-token-for-deferred-charges\n- https://ccbill.com/doc/authenticate-customer-and-create-token-in-one-step\ndescription: CCBill uses OAuth 2.0 client‑credentials flow. Front‑end credentials (Merchant Application ID and Secret Key) are Base64‑encoded\n  and sent with HTTP Basic authentication to obtain an access token, which is then sent as a Bearer token in the Authorization header of API calls.\nschemes:\n- type: http-basic\n  name: Basic\n  evidence: The CCBill RESTful API uses OAuth-based authentication and authorization. Use the frontend credentials ( Merchant Application ID and\n    Secret Key that are Base64 encoded) you received from Merchant Support to generate a frontend\
  \ bearer token .\n  location: header\n  header: Authorization\n  token_url: https://api.ccbill.com/ccbill-auth/oauth/token\n  how_to_obtain: Provide the Frontend_Merchant_Application_ID and Frontend_Secret_Key as the username and password (‑u) in a POST to the token\n    endpoint with grant_type=client_credentials.\n- type: http-bearer\n  name: Bearer\n  evidence: You must include this token in the Authorization header of API requests when creating payment tokens.\n  location: header\n  header: Authorization\n  token_url: https://api.ccbill.com/ccbill-auth/oauth/token\n  how_to_obtain: Use the access token returned from the client_credentials token request as a Bearer token.\ndocs: https://ccbill.com/doc/create-payment-token-non-3ds\n"
source_yaml_url: https://artifacts.apis.io/ccbill/authentication/ccbill-authentication.yml
summary_line: 2 schemes
tags:
- Payments
- Merchant Services
- Billing
- Subscription
- E-Commerce
- Security
---
