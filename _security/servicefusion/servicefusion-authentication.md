---
api_key_in: []
api_specs:
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Customers API
  slug: servicefusion-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Contacts API
  slug: servicefusion-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Jobs API
  slug: servicefusion-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Estimates API
  slug: servicefusion-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Invoices API
  slug: servicefusion-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Products and Services API
  slug: servicefusion-products-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Payments API
  slug: servicefusion-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Techs and Users API
  slug: servicefusion-techs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Calendar Tasks API
  slug: servicefusion-calendar-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Servicefusion Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Service Fusion secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Service Fusion
provider_slug: servicefusion
scheme_count: 2
schemes:
- description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.
  flows:
  - authorizationUrl: https://api.servicefusion.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  name: oauth2
  sources:
  - openapi/servicefusion-openapi.yml
  type: oauth2
- description: Bearer access token obtained via the OAuth 2.0 token endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/servicefusion-openapi.yml
  type: http
slug: servicefusion-authentication
source_filename: servicefusion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/servicefusion-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.servicefusion.com/oauth/authorize\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n    scopes: 0\n  description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.\n  sources:\n  - openapi/servicefusion-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer access token obtained via the OAuth 2.0 token endpoint.\n  sources:\n  - openapi/servicefusion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/authentication/servicefusion-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Field Service Management
- FSM
- Home Services
- Contractors
- Scheduling
- Dispatch
- Invoicing
---
