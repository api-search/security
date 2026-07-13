---
api_key_in:
- header
api_specs:
- filename: tabs-fi-openapi.yml
  format: yaml
  label: Tabs Platform API
  slug: tabs-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs-fi/refs/heads/main/openapi/tabs-fi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tabs Fi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tabs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tabs
provider_slug: tabs-fi
scheme_count: 1
schemes:
- description: Server-side API key issued from the Tabs dashboard for backend integrations.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/tabs-fi-openapi.yml
  type: apiKey
slug: tabs-fi-authentication
source_filename: tabs-fi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tabs-fi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Server-side API key issued from the Tabs dashboard for backend integrations.\n  sources:\n  - openapi/tabs-fi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabs-fi/refs/heads/main/authentication/tabs-fi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Tabs
- Revenue
- Billing
- Invoicing
- Accounts Receivable
- Collections
- Revenue Recognition
- Contracts
- Usage
- Payments
- Subscriptions
- Finance
- B2B
---
