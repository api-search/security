---
api_key_in: []
api_specs:
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Scheduling & Appointments API
  slug: luma-health-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Patients API
  slug: luma-health-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Providers & Facilities API
  slug: luma-health-providers-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Messaging & Engagement API
  slug: luma-health-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Broadcast & Campaigns API
  slug: luma-health-broadcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Intake & Forms API
  slug: luma-health-intake-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Billing & Payments API
  slug: luma-health-billing-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Eligibility & Insurance API
  slug: luma-health-eligibility-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Referrals API
  slug: luma-health-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Conversational AI Assistant API
  slug: luma-health-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Reporting & Audits API
  slug: luma-health-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Authentication API
  slug: luma-health-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Luma Health Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Luma Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Luma Health
provider_slug: luma-health
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: Bearer
  scheme: bearer
  sources:
  - openapi/luma-health-openapi.yaml
  type: http
slug: luma-health-authentication
source_filename: luma-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/luma-health-openapi.yaml\ndocs: https://apidocs.lumahealth.io/#tag/auth\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    Luma Health uses an OAuth2 client-credentials style machine-to-machine flow.\n    A tenant first mints a clientId/clientSecret pair (POST /auth/clients, one\n    active pair per user, rotate with PATCH /auth/clients), then exchanges those\n    credentials for a short-lived JWT access token (POST /auth/token with\n    grant_type=client_credentials). Every other endpoint is then called with\n    Authorization: Bearer <JWT>. The OpenAPI models the applied scheme as an\n    http bearer (JWT) security scheme named \"Bearer\"; there is no scopes surface.\n    Subaccount tokens can also be issued for multi-account tenants.\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/luma-health-openapi.yaml\n\
  token_endpoints:\n- path: /auth/token\n  method: post\n  grant_type: client_credentials\n  request: {client_id, client_secret, grant_type}\n  returns: JWT bearer token\n- path: /auth/clients\n  method: post\n  purpose: Generate clientId/clientSecret (machine-to-machine credentials)\n- path: /auth/clients\n  method: patch\n  purpose: Rotate clientSecret for an existing clientId\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/authentication/luma-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- United States
- Patient Engagement
- Scheduling
- Referrals
- Intake
- Messaging
- Eligibility
- EHR
- Interoperability
- Clinical AI
---
