---
api_key_in: []
api_specs:
- filename: leadiq-data-api-openapi.yml
  format: yaml
  label: LeadIQ Data API
  slug: leadiq-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadiq/refs/heads/main/openapi/leadiq-data-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Leadiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeadIQ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LeadIQ
provider_slug: leadiq
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Use your LeadIQ API key as the username and leave the password empty. API keys are issued in the LeadIQ dashboard under Settings > API Keys.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/leadiq-data-api-openapi.yml
  type: http
slug: leadiq-authentication
source_filename: leadiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/leadiq-data-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Use your LeadIQ API key as the username and leave\n    the password empty. API keys are issued in the LeadIQ dashboard under Settings > API Keys.\n  sources:\n  - openapi/leadiq-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadiq/refs/heads/main/authentication/leadiq-authentication.yml
summary_line: http · 1 scheme
tags:
- Sales Intelligence
- B2B Data
- Contact Data
- Lead Generation
- Prospecting
- CRM Enrichment
- Sales Engagement
- GraphQL
- Model Context Protocol
- Revenue Operations
- Go To Market
---
