---
api_key_in:
- header
api_specs:
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Jobs API
  slug: servicem8-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Job Activities API
  slug: servicem8-job-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Clients (Companies) API
  slug: servicem8-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Job Contacts API
  slug: servicem8-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Staff API
  slug: servicem8-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Materials API
  slug: servicem8-materials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Attachments API
  slug: servicem8-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Queues API
  slug: servicem8-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Vendors API
  slug: servicem8-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Badges API
  slug: servicem8-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Webhooks API
  slug: servicem8-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Servicem8 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ServiceM8 secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ServiceM8
provider_slug: servicem8
scheme_count: 2
schemes:
- description: API key for private/single-account integrations.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/servicem8-openapi.yml
  type: apiKey
- description: OAuth 2.0 for public add-ons. Access tokens expire after 3600 seconds.
  flows:
  - authorizationUrl: https://go.servicem8.com/oauth/authorize
    flow: authorizationCode
    scopes: 11
    tokenUrl: https://go.servicem8.com/oauth/access_token
  name: oauth2
  sources:
  - openapi/servicem8-openapi.yml
  type: oauth2
slug: servicem8-authentication
source_filename: servicem8-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/servicem8-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for private/single-account integrations.\n  sources:\n  - openapi/servicem8-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://go.servicem8.com/oauth/authorize\n    tokenUrl: https://go.servicem8.com/oauth/access_token\n    scopes: 11\n  description: OAuth 2.0 for public add-ons. Access tokens expire after 3600 seconds.\n  sources:\n  - openapi/servicem8-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/authentication/servicem8-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Field Service
- Job Management
- Trades
- Scheduling
- Dispatch
- Invoicing
- Home Services
---
