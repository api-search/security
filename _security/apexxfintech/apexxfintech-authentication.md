---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication is managed using an API key, which is provided to you. Every HTTP call to our API should contain a custom header called X-APIKEY. The value of this header must be the API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Apexxfintech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apexxfintech declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Apexxfintech
provider_slug: apexxfintech
scheme_count: 1
schemes:
- evidence: Authentication is managed using an API key, which is provided to you. Every HTTP call to our API should contain a custom header called X-APIKEY. The value of this header must be the API key.
  header: X-APIKEY
  location: header
  name: X-APIKEY
  type: apiKey
slug: apexxfintech-authentication
source_filename: apexxfintech-authentication.yml
source_heading: Authentication Profile
source_url: https://sandbox.apexx.global/atomic/redoc/api/doc#operation/hostedTokenUsingPOST
source_yaml: "generated: '2026-09-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://sandbox.apexx.global/atomic/redoc/api/doc#operation/hostedTokenUsingPOST\nsources:\n- https://sandbox.apexx.global/atomic/redoc/api/doc#operation/hostedTokenUsingPOST\n- https://sandbox.apexx.global/atomic/redoc/api/doc\ndescription: Authentication is managed using an API key, which is provided to you. Every HTTP call to our API should contain a custom header called\n  X-APIKEY. The value of this header must be the API key.\nschemes:\n- type: apiKey\n  name: X-APIKEY\n  evidence: Authentication is managed using an API key, which is provided to you. Every HTTP call to our API should contain a custom header called\n    X-APIKEY. The value of this header must be the API key.\n  location: header\n  header: X-APIKEY\ndocs: https://sandbox.apexx.global/atomic/redoc/api/doc#operation/hostedTokenUsingPOST\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/authentication/apexxfintech-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- Fintech
- API
- Orchestration
- Global
---
