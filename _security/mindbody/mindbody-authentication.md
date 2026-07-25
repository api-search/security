---
api_key_in:
- header
api_specs:
- filename: mindbody-appointment-api-openapi.yml
  format: yaml
  label: Mindbody Appointment API
  slug: mindbody-appointment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-appointment-api-openapi.yml
- filename: mindbody-class-api-openapi.yml
  format: yaml
  label: Mindbody Class API
  slug: mindbody-class-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-class-api-openapi.yml
- filename: mindbody-client-api-openapi.yml
  format: yaml
  label: Mindbody Client API
  slug: mindbody-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-client-api-openapi.yml
- filename: mindbody-cross-site-api-openapi.yml
  format: yaml
  label: Mindbody Cross Site API
  slug: mindbody-cross-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-cross-site-api-openapi.yml
- filename: mindbody-enrollment-api-openapi.yml
  format: yaml
  label: Mindbody Enrollment API
  slug: mindbody-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-enrollment-api-openapi.yml
- filename: mindbody-metrics-api-openapi.yml
  format: yaml
  label: Mindbody Metrics API
  slug: mindbody-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-metrics-api-openapi.yml
- filename: mindbody-payroll-api-openapi.yml
  format: yaml
  label: Mindbody Payroll API
  slug: mindbody-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-payroll-api-openapi.yml
- filename: mindbody-pick-a-spot-api-openapi.yml
  format: yaml
  label: Mindbody Pick A Spot API
  slug: mindbody-pick-a-spot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-pick-a-spot-api-openapi.yml
- filename: mindbody-sale-api-openapi.yml
  format: yaml
  label: Mindbody Sale API
  slug: mindbody-sale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-sale-api-openapi.yml
- filename: mindbody-site-api-openapi.yml
  format: yaml
  label: Mindbody Site API
  slug: mindbody-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-site-api-openapi.yml
- filename: mindbody-staff-api-openapi.yml
  format: yaml
  label: Mindbody Staff API
  slug: mindbody-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-staff-api-openapi.yml
- filename: mindbody-subscriptions-api-openapi.yml
  format: yaml
  label: Mindbody Subscriptions API
  slug: mindbody-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-subscriptions-api-openapi.yml
- filename: mindbody-user-token-api-openapi.yml
  format: yaml
  label: Mindbody User Token API
  slug: mindbody-user-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/openapi/mindbody-user-token-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Mindbody Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Mindbody secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Mindbody
provider_slug: mindbody
scheme_count: 2
schemes:
- description: Mindbody-issued API key (server-to-server). Required on every request.
  in: header
  name: ApiKeyAuth
  parameter: API-Key
  sources:
  - openapi/mindbody-public-api-v6-openapi-original.yml
  - openapi/mindbody-webhooks-api-openapi-original.yml
  type: apiKey
- description: OpenID Connect bearer token issued by Mindbody Identity Service (signin.mindbodyonline.com). Required for endpoints that act on behalf of a staff or client user.
  flows:
  - authorizationUrl: https://signin.mindbodyonline.com/connect/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://signin.mindbodyonline.com/connect/token
  name: OAuth2
  sources:
  - openapi/mindbody-public-api-v6-openapi-original.yml
  type: oauth2
slug: mindbody-authentication
source_filename: mindbody-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mindbody-public-api-v6-openapi-original.yml, openapi/mindbody-webhooks-api-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: API-Key\n  description: Mindbody-issued API key (server-to-server). Required on every request.\n  sources:\n  - openapi/mindbody-public-api-v6-openapi-original.yml\n  - openapi/mindbody-webhooks-api-openapi-original.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://signin.mindbodyonline.com/connect/authorize\n    tokenUrl: https://signin.mindbodyonline.com/connect/token\n    scopes: 5\n  description: OpenID Connect bearer token issued by Mindbody Identity Service (signin.mindbodyonline.com).\n    Required for endpoints that act on behalf of a staff or client user.\n  sources:\n  - openapi/mindbody-public-api-v6-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/authentication/mindbody-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Fitness
- Wellness
- Beauty
- Scheduling
- Booking
- Point of Sale
- Studios
- Salons
- Spas
- Webhooks
---
