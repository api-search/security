---
api_key_in:
- header
api_specs:
- filename: adapt-prospect-api-openapi.yml
  format: yaml
  label: Adapt Prospect API
  slug: adapt-prospect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapt-io/refs/heads/main/openapi/adapt-prospect-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
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
  - openapi/adapt-prospect-api-openapi.yml
  type: apiKey
- description: API key from the Adapt account settings page.
  in: header
  name: apiKeyAuth
  parameter: apiKey
  sources:
  - openapi/adapt-prospect-api-openapi.yml
  type: apiKey
slug: adapt-io-authentication
source_filename: adapt-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adapt-prospect-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: emailAuth\n  type: apiKey\n  in: header\n  parameter: email\n  description: Account email used to register with Adapt.\n  sources:\n  - openapi/adapt-prospect-api-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: API key from the Adapt account settings page.\n  sources:\n  - openapi/adapt-prospect-api-openapi.yml\n"
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
- ABM
- CRM Enrichment
- Marketing
- Sales
---
