---
api_key_in: []
api_specs:
- filename: forter-openapi.yml
  format: yaml
  label: Forter Order Decision API
  slug: forter-order-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/openapi/forter-openapi.yml
- filename: forter-openapi.yml
  format: yaml
  label: Forter Account Protection API
  slug: forter-account-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/openapi/forter-openapi.yml
- filename: forter-openapi.yml
  format: yaml
  label: Forter Chargeback and Compensation API
  slug: forter-chargeback-compensation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/openapi/forter-openapi.yml
- filename: forter-openapi.yml
  format: yaml
  label: Forter Data Privacy API
  slug: forter-data-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/openapi/forter-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Forter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Forter
provider_slug: forter
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication with your Forter API key as the username (empty password). Requests must also carry the `x-forter-siteid` header (your site ID), an `api-version` header (for example `10.1`), and `Content-Type: application/json`. The site ID and API key are provisioned by Forter during enterprise onboarding and are found in your account credentials. Requests are sent to a per-tenant host by prepending the site ID to the API host (https://{siteId}.api.forter.secure.com).'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/forter-openapi.yml
  - https://docs.forter.com/docs/api-overview
  type: http
slug: forter-authentication
source_filename: forter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/forter-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication with your Forter API key as the username (empty\n    password). Requests must also carry the `x-forter-siteid` header (your site\n    ID), an `api-version` header (for example `10.1`), and\n    `Content-Type: application/json`. The site ID and API key are provisioned by\n    Forter during enterprise onboarding and are found in your account\n    credentials. Requests are sent to a per-tenant host by prepending the site\n    ID to the API host (https://{siteId}.api.forter.secure.com).\n  sources:\n  - openapi/forter-openapi.yml\n  - https://docs.forter.com/docs/api-overview\nnotes: >-\n  Forter's Tokenization API additionally supports HMAC request signing (SHA256,\n  SHA512, SHA1, MD5), IP allow-listing, target-URL allow-listing, and mTLS. The\n  Core order/account/decision\
  \ endpoints modeled in this catalog entry use Basic\n  auth plus the site-ID header, per docs.forter.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/authentication/forter-authentication.yml
summary_line: http · 1 scheme
tags:
- Fraud Detection
- Fraud Prevention
- Identity
- Trust
- Payments
- Chargebacks
- Account Protection
- E-commerce
- Risk
- Machine Learning
---
