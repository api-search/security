---
api_key_in: []
api_specs:
- filename: uncapped-applicants-api-openapi.yml
  format: yaml
  label: Uncapped Applicants API
  slug: uncapped-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uncapped/refs/heads/main/openapi/uncapped-applicants-api-openapi.yml
- filename: uncapped-applications-api-openapi.yml
  format: yaml
  label: Uncapped Applications API
  slug: uncapped-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uncapped/refs/heads/main/openapi/uncapped-applications-api-openapi.yml
- filename: uncapped-authentication-api-openapi.yml
  format: yaml
  label: Uncapped Authentication API
  slug: uncapped-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uncapped/refs/heads/main/openapi/uncapped-authentication-api-openapi.yml
- filename: uncapped-estimations-api-openapi.yml
  format: yaml
  label: Uncapped Estimations API
  slug: uncapped-estimations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uncapped/refs/heads/main/openapi/uncapped-estimations-api-openapi.yml
- filename: uncapped-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Uncapped Webhook Subscriptions API
  slug: uncapped-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uncapped/refs/heads/main/openapi/uncapped-webhook-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Uncapped Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uncapped secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uncapped
provider_slug: uncapped
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: auth0_bearer
  scheme: bearer
  sources:
  - openapi/uncapped-partners-openapi-original.json
  type: http
slug: uncapped-authentication
source_filename: uncapped-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/uncapped-partners-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: auth0_bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/uncapped-partners-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uncapped/refs/heads/main/authentication/uncapped-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Lending
- Embedded Finance
- Revenue-Based Financing
- Working Capital
- E-Commerce
---
