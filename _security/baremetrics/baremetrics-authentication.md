---
api_key_in:
- header
api_specs:
- filename: baremetrics-annotations-api-openapi.yml
  format: yaml
  label: Baremetrics Annotations API
  slug: baremetrics-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baremetrics/refs/heads/main/openapi/baremetrics-annotations-api-openapi.yml
- filename: baremetrics-charges-api-openapi.yml
  format: yaml
  label: Baremetrics Charges API
  slug: baremetrics-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baremetrics/refs/heads/main/openapi/baremetrics-charges-api-openapi.yml
- filename: baremetrics-customers-api-openapi.yml
  format: yaml
  label: Baremetrics Customers API
  slug: baremetrics-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baremetrics/refs/heads/main/openapi/baremetrics-customers-api-openapi.yml
- filename: baremetrics-events-api-openapi.yml
  format: yaml
  label: Baremetrics Events API
  slug: baremetrics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baremetrics/refs/heads/main/openapi/baremetrics-events-api-openapi.yml
- filename: baremetrics-metrics-api-openapi.yml
  format: yaml
  label: Baremetrics Metrics API
  slug: baremetrics-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baremetrics/refs/heads/main/openapi/baremetrics-metrics-api-openapi.yml
- filename: baremetrics-plans-api-openapi.yml
  format: yaml
  label: Baremetrics Plans API
  slug: baremetrics-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baremetrics/refs/heads/main/openapi/baremetrics-plans-api-openapi.yml
- filename: baremetrics-subscriptions-api-openapi.yml
  format: yaml
  label: Baremetrics Subscriptions API
  slug: baremetrics-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baremetrics/refs/heads/main/openapi/baremetrics-subscriptions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Baremetrics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Baremetrics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Baremetrics
provider_slug: baremetrics
scheme_count: 1
schemes:
- in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/baremetrics-openapi.json
  type: apiKey
slug: baremetrics-authentication
source_filename: baremetrics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/baremetrics-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/baremetrics-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baremetrics/refs/heads/main/authentication/baremetrics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Subscription Analytics
- MRR
- ARR
- Churn Rate
- LTV
- Revenue
- Stripe
- Financial Metrics
- Software-as-a-Service
---
