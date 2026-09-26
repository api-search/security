---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication requires generating a hashed message authentication code (HMAC-SHA256).
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Autoservicefinancelimited Authentication
name_suffix: Authentication
oauth_flows: []
overview: Autoservicefinancelimited declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Autoservicefinancelimited
provider_slug: autoservicefinancelimited
scheme_count: 1
schemes:
- evidence: Authentication requires generating a hashed message authentication code (HMAC-SHA256).
  how_to_obtain: A secret is provided by BUMPER and used to compute the signature hash; the api_key is supplier‑specific and provided by BUMPER.
  location: body
  name: HMAC-SHA256
  type: hmac
slug: autoservicefinancelimited-authentication
source_filename: autoservicefinancelimited-authentication.yml
source_heading: Authentication Profile
source_url: https://api-docs.bumper.co/bumper-api-documentation/authentication.md
source_yaml: "generated: '2026-09-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api-docs.bumper.co/bumper-api-documentation/authentication.md\nsources:\n- https://api-docs.bumper.co/bumper-api-documentation/authentication.md\n- https://api-docs.bumper.co/bumper-api-documentation/reference/payment-solutions/payplus-subscriptions/setup-subscription.md\n- https://api-docs.bumper.co/bumper-api-documentation/reference/payment-solutions/payplus-subscriptions/setup-subscription/example-request.md\ndescription: Authentication requires generating a hashed message authentication code (HMAC-SHA256).\nschemes:\n- type: hmac\n  name: HMAC-SHA256\n  evidence: Authentication requires generating a hashed message authentication code (HMAC-SHA256).\n  location: body\n  how_to_obtain: A secret is provided by BUMPER and used to compute the signature hash; the api_key is supplier‑specific and provided by BUMPER.\nnote: The signature and api_key are included in the request\
  \ body as shown in the example payloads.\ndocs: https://api-docs.bumper.co/bumper-api-documentation/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autoservicefinancelimited/refs/heads/main/authentication/autoservicefinancelimited-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Automotive
- FinTech
- UK
- Payments
---
