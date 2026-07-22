---
api_key_in:
- header
api_specs:
- filename: persistiq-openapi.yml
  format: yaml
  label: PersistIQ API
  slug: persistiq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/openapi/persistiq-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Persistiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: PersistIQ secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PersistIQ
provider_slug: persistiq
scheme_count: 1
schemes:
- description: Company-wide API key. Grants access to read and write all users' data within the company. Include it in the header of every request.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/persistiq-openapi.yml
  type: apiKey
slug: persistiq-authentication
source_filename: persistiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/persistiq-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Company-wide API key. Grants access to read and write all users' data within\n    the company. Include it in the header of every request.\n  sources:\n  - openapi/persistiq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/authentication/persistiq-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Sales Engagement
- Sales
- Outbound
- Email Outreach
- CRM
- Lead Management
- Marketing
---
