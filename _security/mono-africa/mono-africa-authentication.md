---
api_key_in: []
api_specs:
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Connect API
  slug: mono-africa-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Financial Data API
  slug: mono-africa-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Investment Data API
  slug: mono-africa-investment-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Creditworthiness API
  slug: mono-africa-creditworthiness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono DirectPay API
  slug: mono-africa-directpay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Lookup API
  slug: mono-africa-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mono Africa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mono secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mono
provider_slug: mono-africa
scheme_count: 1
schemes:
- description: Secret key for the Mono application, obtained self-serve from the Mono dashboard. Sent on every server-to-server request in the `mono-sec-key` header. Applications have separate test and live secret keys; use test keys against the sandbox and live keys in production. The public key is used only by the front-end Connect / DirectPay widgets, never for server API calls.
  in: header
  keyName: mono-sec-key
  name: monoSecKey
  sources:
  - openapi/mono-africa-openapi.yml
  - https://docs.mono.co/docs/quickstart
  type: apiKey
slug: mono-africa-authentication
source_filename: mono-africa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/mono-africa-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: monoSecKey\n  type: apiKey\n  in: header\n  keyName: mono-sec-key\n  description: >-\n    Secret key for the Mono application, obtained self-serve from the Mono\n    dashboard. Sent on every server-to-server request in the `mono-sec-key`\n    header. Applications have separate test and live secret keys; use test keys\n    against the sandbox and live keys in production. The public key is used only\n    by the front-end Connect / DirectPay widgets, never for server API calls.\n  sources:\n  - openapi/mono-africa-openapi.yml\n  - https://docs.mono.co/docs/quickstart\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/authentication/mono-africa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Open Banking
- Financial Data
- Payments
- Fintech
- Account Linking
- Direct Debit
- Bank Data
- Africa
- Nigeria
- Financial Infrastructure
---
