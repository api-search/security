---
api_key_in: []
api_specs:
- filename: hawksoft-openapi.yml
  format: yaml
  label: HawkSoft Agencies and Offices API
  slug: hawksoft-agencies-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/openapi/hawksoft-openapi.yml
- filename: hawksoft-openapi.yml
  format: yaml
  label: HawkSoft Clients API
  slug: hawksoft-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/openapi/hawksoft-openapi.yml
- filename: hawksoft-openapi.yml
  format: yaml
  label: HawkSoft Log Entries API
  slug: hawksoft-log-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/openapi/hawksoft-openapi.yml
- filename: hawksoft-openapi.yml
  format: yaml
  label: HawkSoft Attachments and Receipts API
  slug: hawksoft-attachments-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/openapi/hawksoft-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hawksoft Authentication
name_suffix: Authentication
oauth_flows: []
overview: HawkSoft secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HawkSoft
provider_slug: hawksoft
scheme_count: 1
schemes:
- description: HTTP Basic authentication with partner-issued credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/hawksoft-openapi.yml
  type: http
slug: hawksoft-authentication
source_filename: hawksoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hawksoft-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with partner-issued credentials.\n  sources:\n  - openapi/hawksoft-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/authentication/hawksoft-authentication.yml
summary_line: http · 1 scheme
tags:
- Insurance
- Agency Management System
- AMS
- InsurTech
- Property and Casualty
- Partner API
- Gated API
---
