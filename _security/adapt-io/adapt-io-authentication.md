---
api_key_in:
- header
api_specs:
- filename: adapt-io-company-search-api-openapi.yml
  format: yaml
  label: Adapt Company Search API
  slug: adapt-io-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapt-io/refs/heads/main/openapi/adapt-io-company-search-api-openapi.yml
- filename: adapt-io-contact-enrichment-api-openapi.yml
  format: yaml
  label: Adapt Contact Enrichment API
  slug: adapt-io-contact-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapt-io/refs/heads/main/openapi/adapt-io-contact-enrichment-api-openapi.yml
- filename: adapt-io-contact-purchase-api-openapi.yml
  format: yaml
  label: Adapt Contact Purchase API
  slug: adapt-io-contact-purchase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapt-io/refs/heads/main/openapi/adapt-io-contact-purchase-api-openapi.yml
- filename: adapt-io-contact-search-api-openapi.yml
  format: yaml
  label: Adapt Contact Search API
  slug: adapt-io-contact-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapt-io/refs/heads/main/openapi/adapt-io-contact-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Adapt Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adapt secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adapt
provider_slug: adapt-io
scheme_count: 2
schemes:
- description: Account email used to register with Adapt.
  in: header
  name: emailAuth
  parameter: email
  sources:
  - openapi/adapt-io-company-search-api-openapi.yml
  - openapi/adapt-io-contact-enrichment-api-openapi.yml
  - openapi/adapt-io-contact-purchase-api-openapi.yml
  - openapi/adapt-io-contact-search-api-openapi.yml
  type: apiKey
- description: API key from the Adapt account settings page.
  in: header
  name: apiKeyAuth
  parameter: apiKey
  sources:
  - openapi/adapt-io-company-search-api-openapi.yml
  - openapi/adapt-io-contact-enrichment-api-openapi.yml
  - openapi/adapt-io-contact-purchase-api-openapi.yml
  - openapi/adapt-io-contact-search-api-openapi.yml
  type: apiKey
slug: adapt-io-authentication
source_filename: adapt-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.adapt.io/api-docs/v3/\ndocs: https://www.adapt.io/api-docs/v3/\nderived_from: openapi/adapt-io-company-search-api-openapi.yml, openapi/adapt-io-contact-enrichment-api-openapi.yml,\n  openapi/adapt-io-contact-purchase-api-openapi.yml, openapi/adapt-io-contact-search-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth: false\n  openid_connect: false\n  mutual_tls: false\n  bearer: false\n  schemes_required_together: true\ncredentials:\n  issuance: >-\n    Keys are issued in the Adapt web app account settings page. There is no key-management\n    API and no programmatic key rotation.\n  management_url: https://leads.adapt.io/profile/settings\n  gated: true\n  gate: >-\n    API access is available on Adapt's Custom (enterprise) plan only. Free, Starter and\n    Basic tiers do not expose Prospect API credentials — an account without API access\n    fails with APP-403-002 (\"You don't have\
  \ access to this API\"), and an account with no\n    subscription fails with APP-403-001.\n  rotation_policy: not published\n  expiry: not published\n  scopes: none — the key carries full account privileges across all four operations\ntransport:\n  https_required: true\n  evidence: >-\n    \"All of Adapt's APIs are organized around REST, and all requests must be made over\n    SSL.\" — https://www.adapt.io/api-docs/v3/\nfindings:\n  - >-\n    Both headers must be sent together on every request; either one alone fails with\n    APP-401-001. This is unusual — the account identifier travels in a header named\n    `email` rather than being encoded in the key itself.\n  - >-\n    Neither header uses a conventional name (`Authorization`, `X-API-Key`), so generic\n    API clients, gateways and agent runtimes will not pick the credentials up from a\n    standard auth configuration.\n  - >-\n    A single credential pair grants every operation including the credit-spending\n    purchase call. There\
  \ is no read-only key, no scoping, and no documented rotation or\n    expiry, so a leaked key can drain an account's email and phone credits.\nschemes:\n- name: emailAuth\n  type: apiKey\n  in: header\n  parameter: email\n  description: Account email used to register with Adapt.\n  sources:\n  - openapi/adapt-io-company-search-api-openapi.yml\n  - openapi/adapt-io-contact-enrichment-api-openapi.yml\n  - openapi/adapt-io-contact-purchase-api-openapi.yml\n  - openapi/adapt-io-contact-search-api-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: API key from the Adapt account settings page.\n  sources:\n  - openapi/adapt-io-company-search-api-openapi.yml\n  - openapi/adapt-io-contact-enrichment-api-openapi.yml\n  - openapi/adapt-io-contact-purchase-api-openapi.yml\n  - openapi/adapt-io-contact-search-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adapt-io/refs/heads/main/authentication/adapt-io-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- B2B Data
- Contact Data
- Company Data
- Lead Intelligence
- Sales Intelligence
- Sales Acceleration
- Data Enrichment
- Prospecting
- Lead Generation
- Email Finder
- Account Based Marketing
- CRM Enrichment
- Marketing
- Sales
---
