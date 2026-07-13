---
api_key_in: []
api_specs:
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Home Services Estimate API
  slug: taskrabbit-home-services-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Home Services Availability API
  slug: taskrabbit-home-services-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Home Services Booking API
  slug: taskrabbit-home-services-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Home Services Catalog API
  slug: taskrabbit-home-services-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
- filename: taskrabbit-openapi.yml
  format: yaml
  label: TaskRabbit Delivery API (Dolly)
  slug: taskrabbit-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/openapi/taskrabbit-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Taskrabbit Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: TaskRabbit secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: TaskRabbit
provider_slug: taskrabbit
scheme_count: 1
schemes:
- description: Auth0 machine-to-machine (M2M) OAuth2 client-credentials grant. Credentials are issued during partner onboarding.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://taskrabbit.auth0.com/oauth/token
  name: oauth2
  sources:
  - openapi/taskrabbit-openapi.yml
  type: oauth2
slug: taskrabbit-authentication
source_filename: taskrabbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/taskrabbit-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://taskrabbit.auth0.com/oauth/token\n    scopes: 0\n  description: Auth0 machine-to-machine (M2M) OAuth2 client-credentials grant. Credentials are\n    issued during partner onboarding.\n  sources:\n  - openapi/taskrabbit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskrabbit/refs/heads/main/authentication/taskrabbit-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Gig Economy
- Handyman
- Home Services
- Marketplace
- Delivery
- Moving
- Partner API
- IKEA
---
