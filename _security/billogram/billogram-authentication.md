---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Billogram Authentication
name_suffix: Authentication
oauth_flows: []
overview: Billogram secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Billogram
provider_slug: billogram
scheme_count: 1
schemes:
- credential_source: Created in the Billogram web app under Company Settings -> API -> API Users. Separate API users are recommended per integration for independent access management.
  description: 'HTTP Basic Authentication. The API User ID is sent as the username and the API Key as the password, Base64-encoded in the Authorization header (Authorization: Basic base64(API_USER_ID:API_KEY)). All requests must be made over HTTPS.'
  environment_separation: Credentials are environment-specific; sandbox credentials only work against the sandbox base URL and production credentials only against production.
  environments:
    production: https://billogram.com/api/v2
    sandbox: https://sandbox.billogram.com/api/v2
  name: basicAuth
  scheme: basic
  type: http
slug: billogram-authentication
source_filename: billogram-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.billogram.com/guides/authentication\ndocs: https://docs.billogram.com/guides/authentication\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  transport: https-required\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic Authentication. The API User ID is sent as the username and the\n    API Key as the password, Base64-encoded in the Authorization header\n    (Authorization: Basic base64(API_USER_ID:API_KEY)). All requests must be\n    made over HTTPS.\n  credential_source: >-\n    Created in the Billogram web app under Company Settings -> API -> API Users.\n    Separate API users are recommended per integration for independent access\n    management.\n  environments:\n    sandbox: https://sandbox.billogram.com/api/v2\n    production: https://billogram.com/api/v2\n  environment_separation: >-\n    Credentials are environment-specific; sandbox credentials only work\
  \ against\n    the sandbox base URL and production credentials only against production.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billogram/refs/heads/main/authentication/billogram-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Applicative Saas
- Invoicing
- Billing
- Payments
- Invoice-to-Cash
- E-invoicing
- Fintech
- Webhooks
---
