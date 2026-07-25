---
api_key_in: []
api_specs:
- filename: snov-io-authentication-api-openapi.yml
  format: yaml
  label: Snov.io Authentication API
  slug: snov-io-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-authentication-api-openapi.yml
- filename: snov-io-campaigns-api-openapi.yml
  format: yaml
  label: Snov.io Campaigns API
  slug: snov-io-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-campaigns-api-openapi.yml
- filename: snov-io-crm-pipeline-api-openapi.yml
  format: yaml
  label: Snov.io CRM Pipeline API
  slug: snov-io-crm-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-crm-pipeline-api-openapi.yml
- filename: snov-io-domain-search-api-openapi.yml
  format: yaml
  label: Snov.io Domain Search API
  slug: snov-io-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-domain-search-api-openapi.yml
- filename: snov-io-email-accounts-api-openapi.yml
  format: yaml
  label: Snov.io Email Accounts API
  slug: snov-io-email-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-accounts-api-openapi.yml
- filename: snov-io-email-finder-api-openapi.yml
  format: yaml
  label: Snov.io Email Finder API
  slug: snov-io-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-finder-api-openapi.yml
- filename: snov-io-email-verification-api-openapi.yml
  format: yaml
  label: Snov.io Email Verification API
  slug: snov-io-email-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-verification-api-openapi.yml
- filename: snov-io-email-warm-up-api-openapi.yml
  format: yaml
  label: Snov.io Email Warm-up API
  slug: snov-io-email-warm-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-warm-up-api-openapi.yml
- filename: snov-io-prospects-api-openapi.yml
  format: yaml
  label: Snov.io Prospects API
  slug: snov-io-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-prospects-api-openapi.yml
- filename: snov-io-user-api-openapi.yml
  format: yaml
  label: Snov.io User API
  slug: snov-io-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-user-api-openapi.yml
- filename: snov-io-webhooks-api-openapi.yml
  format: yaml
  label: Snov.io Webhooks API
  slug: snov-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Snov Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snov.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Snov.io
provider_slug: snov-io
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Obtain a Bearer token via POST /v1/oauth/access_token using client credentials. Tokens expire after 3600 seconds.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/snov-io-openapi.yml
  type: http
slug: snov-io-authentication
source_filename: snov-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snov-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Obtain a Bearer token via POST /v1/oauth/access_token using client credentials.\n    Tokens expire after 3600 seconds.\n  sources:\n  - openapi/snov-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/authentication/snov-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Sales Automation
- Email Finder
- Email Verification
- Lead Generation
- Drip Campaigns
- CRM
- LinkedIn Automation
- Prospect Management
- Data Enrichment
- Cold Email
---
