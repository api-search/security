---
api_key_in: []
api_specs:
- filename: snov-io-openapi.yml
  format: yaml
  label: Snov.io Email Finder API
  slug: snovio-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-openapi.yml
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
