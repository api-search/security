---
api_key_in: []
api_specs:
- filename: paigo-customers-api-openapi.yml
  format: yaml
  label: Paigo Customers API
  slug: paigo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-customers-api-openapi.yml
- filename: paigo-dimensions-api-openapi.yml
  format: yaml
  label: Paigo Dimensions API
  slug: paigo-dimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-dimensions-api-openapi.yml
- filename: paigo-invoices-api-openapi.yml
  format: yaml
  label: Paigo Invoices API
  slug: paigo-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-invoices-api-openapi.yml
- filename: paigo-measurements-api-openapi.yml
  format: yaml
  label: Paigo Measurements API
  slug: paigo-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-measurements-api-openapi.yml
- filename: paigo-offerings-api-openapi.yml
  format: yaml
  label: Paigo Offerings API
  slug: paigo-offerings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-offerings-api-openapi.yml
- filename: paigo-settings-api-openapi.yml
  format: yaml
  label: Paigo Settings API
  slug: paigo-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-settings-api-openapi.yml
- filename: paigo-usage-api-openapi.yml
  format: yaml
  label: Paigo Usage API
  slug: paigo-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-usage-api-openapi.yml
- filename: paigo-webhooks-api-openapi.yml
  format: yaml
  label: Paigo Webhooks API
  slug: paigo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Paigo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Paigo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Paigo
provider_slug: paigo
scheme_count: 1
schemes:
- description: Use bearer token to authenticate `Bearer <your access token>`
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.paigo.tech/oauth/token
  name: bearer
  sources:
  - openapi/paigo-paigo-api-openapi.yml
  type: oauth2
slug: paigo-authentication
source_filename: paigo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paigo-paigo-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearer\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.paigo.tech/oauth/token\n    scopes: 0\n  description: Use bearer token to authenticate `Bearer <your access token>`\n  sources:\n  - openapi/paigo-paigo-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/authentication/paigo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Billing
- Usage-Based Billing
- Metering
- Invoicing
- Pricing
- Software-as-a-Service
- Subscription
- Developer Tools
- FinOps
---
