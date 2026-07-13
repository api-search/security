---
api_key_in:
- header
api_specs:
- filename: buildxact-public-api-openapi.yml
  format: yaml
  label: Buildxact Public API
  slug: buildxact-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildxact/refs/heads/main/openapi/buildxact-public-api-openapi.yml
- filename: buildxact-webhooks-asyncapi.yml
  format: yaml
  label: Buildxact Webhooks
  slug: buildxact-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildxact/refs/heads/main/asyncapi/buildxact-webhooks-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Buildxact Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buildxact secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Buildxact
provider_slug: buildxact
scheme_count: 2
schemes:
- description: Azure API Management subscription key issued to a partner organization.
  in: header
  name: SubscriptionKey
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/buildxact-public-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Short-lived bearer token obtained from /accounts/auth/login.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/buildxact-public-api-openapi.yml
  type: http
slug: buildxact-authentication
source_filename: buildxact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/buildxact-public-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: SubscriptionKey\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: Azure API Management subscription key issued to a partner organization.\n  sources:\n  - openapi/buildxact-public-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Short-lived bearer token obtained from /accounts/auth/login.\n  sources:\n  - openapi/buildxact-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildxact/refs/heads/main/authentication/buildxact-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Construction
- Residential Construction
- Construction Management
- Estimating
- Takeoffs
- Job Management
- Project Management
- Quoting
- Scheduling
- Purchase Orders
- Invoicing
- Supplier Integration
- Material Pricing
- Builders
- Remodelers
- Trades
- SaaS
- Australia
- Autodesk
---
