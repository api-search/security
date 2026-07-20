---
api_key_in:
- header
api_specs:
- filename: figure-heloc-inquiries-openapi-original.yml
  format: yaml
  label: HELOC Inquiries
  slug: heloc-inquiries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure/refs/heads/main/openapi/figure-heloc-inquiries-openapi-original.yml
- filename: figure-heloc-pre-qualification-openapi-original.yml
  format: yaml
  label: HELOC Pre-qualification
  slug: heloc-pre-qualification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure/refs/heads/main/openapi/figure-heloc-pre-qualification-openapi-original.yml
- filename: figure-portfolio-manager-openapi-original.yml
  format: yaml
  label: Portfolio Manager
  slug: portfolio-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure/refs/heads/main/openapi/figure-portfolio-manager-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Figure Authentication
name_suffix: Authentication
oauth_flows: []
overview: Figure secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Figure
provider_slug: figure
scheme_count: 1
schemes:
- applies_to:
  - HELOC Inquiries
  - HELOC Pre-qualification
  - Portfolio Manager
  in: header
  name: apikey
  parameter: apikey
  sources:
  - openapi/figure-heloc-inquiries-openapi-original.yml
  type: apiKey
slug: figure-authentication
source_filename: figure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/figure-heloc-inquiries-openapi-original.yml\ndocs: https://docs.figure.com/getting-started\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    All Figure Partner APIs (HELOC Inquiries, HELOC Pre-qualification, Portfolio\n    Manager) authenticate with a single apikey request header. Keys are issued\n    per environment (test vs production) during onboarding. A User-Agent header\n    is also required on every request. Payloads may be optionally JWE/RSA-encrypted:\n    requests encrypted with Figure's public key, responses encrypted on demand via\n    the X-Encrypt-Response: true header. No OAuth2/OIDC is used, so there is no scope\n    surface.\n  jwe_encryption: https://docs.figure.com/jwe-data-protection/intro\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/figure-heloc-inquiries-openapi-original.yml\n  applies_to:\n  - HELOC Inquiries\n\
  \  - HELOC Pre-qualification\n  - Portfolio Manager\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figure/refs/heads/main/authentication/figure-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Lending
- HELOC
- Home Equity
- Mortgage
- Loan Origination
- Webhooks
- Capital Markets
---
