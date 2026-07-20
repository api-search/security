---
api_key_in: []
api_specs:
- filename: enrich-so-openapi.yml
  format: yaml
  label: Enrich Person Enrichment API
  slug: enrich-so-person-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-openapi.yml
- filename: enrich-so-openapi.yml
  format: yaml
  label: Enrich Email Finder API
  slug: enrich-so-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-openapi.yml
- filename: enrich-so-openapi.yml
  format: yaml
  label: Enrich Email Verification API
  slug: enrich-so-email-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-openapi.yml
- filename: enrich-so-openapi.yml
  format: yaml
  label: Enrich Phone Finder API
  slug: enrich-so-phone-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-openapi.yml
- filename: enrich-so-openapi.yml
  format: yaml
  label: Enrich Company Intelligence API
  slug: enrich-so-company-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-openapi.yml
- filename: enrich-so-openapi.yml
  format: yaml
  label: Enrich Lead Finder API
  slug: enrich-so-lead-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Enrich So Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enrich secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Enrich
provider_slug: enrich-so
scheme_count: 2
schemes:
- description: API key passed in the x-api-key header (recommended). Keys are created and managed in the Enrich dashboard at https://dash.enrich.so/dashboard/api-keys and are prefixed with sk_ (for example sk_prod_...). A missing, invalid, or disabled key returns 401.
  in: header
  keyName: x-api-key
  name: apiKeyHeader
  sources:
  - https://doc.enrich.so/authentication-1951026m0
  - openapi/enrich-so-openapi.yml
  type: apiKey
- description: 'The same API key may alternatively be sent as an Authorization Bearer token (Authorization: Bearer [example key]).'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://doc.enrich.so/authentication-1951026m0
  - openapi/enrich-so-openapi.yml
  type: http
slug: enrich-so-authentication
source_filename: enrich-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/enrich-so-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  keyName: x-api-key\n  description: >-\n    API key passed in the x-api-key header (recommended). Keys are created and managed in\n    the Enrich dashboard at https://dash.enrich.so/dashboard/api-keys and are prefixed with\n    sk_ (for example sk_prod_...). A missing, invalid, or disabled key returns 401.\n  sources:\n  - https://doc.enrich.so/authentication-1951026m0\n  - openapi/enrich-so-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    The same API key may alternatively be sent as an Authorization Bearer token\n    (Authorization: Bearer [example key]).\n  sources:\n  - https://doc.enrich.so/authentication-1951026m0\n  - openapi/enrich-so-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/authentication/enrich-so-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Data Enrichment
- Contact Discovery
- Web Intelligence
- B2B Data
- Lead Enrichment
- Email Finder
- Email Verification
- Phone Numbers
- LinkedIn
- Reference Data
---
