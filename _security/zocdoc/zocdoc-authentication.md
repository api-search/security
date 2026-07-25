---
api_key_in: []
api_specs:
- filename: zocdoc-appointments-api-openapi.yml
  format: yaml
  label: Zocdoc appointments API
  slug: zocdoc-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-appointments-api-openapi.yml
- filename: zocdoc-calendar-integration-timeslots-api-openapi.yml
  format: yaml
  label: Zocdoc calendar-integration-timeslots API
  slug: zocdoc-calendar-integration-timeslots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml
- filename: zocdoc-credentials-api-openapi.yml
  format: yaml
  label: Zocdoc credentials API
  slug: zocdoc-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-credentials-api-openapi.yml
- filename: zocdoc-facilities-api-openapi.yml
  format: yaml
  label: Zocdoc facilities API
  slug: zocdoc-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-facilities-api-openapi.yml
- filename: zocdoc-insurance-reference-api-openapi.yml
  format: yaml
  label: Zocdoc insurance-reference API
  slug: zocdoc-insurance-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-insurance-reference-api-openapi.yml
- filename: zocdoc-provider-locations-api-openapi.yml
  format: yaml
  label: Zocdoc provider-locations API
  slug: zocdoc-provider-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-provider-locations-api-openapi.yml
- filename: zocdoc-providers-api-openapi.yml
  format: yaml
  label: Zocdoc providers API
  slug: zocdoc-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-providers-api-openapi.yml
- filename: zocdoc-reference-api-openapi.yml
  format: yaml
  label: Zocdoc reference API
  slug: zocdoc-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-reference-api-openapi.yml
- filename: zocdoc-schedulable-entities-api-openapi.yml
  format: yaml
  label: Zocdoc schedulable-entities API
  slug: zocdoc-schedulable-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-schedulable-entities-api-openapi.yml
- filename: zocdoc-webhook-api-openapi.yml
  format: yaml
  label: Zocdoc webhook API
  slug: zocdoc-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-webhook-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zocdoc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Zocdoc secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Zocdoc
provider_slug: zocdoc
scheme_count: 2
schemes:
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    scopes: 6
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  sources:
  - openapi/zocdoc-zocdoc-api-openapi.yml
  type: oauth2
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  sources:
  - openapi/zocdoc-zocdoc-api-openapi.yml
  type: oauth2
slug: zocdoc-authentication
source_filename: zocdoc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zocdoc-zocdoc-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: ClientCredentialsFlow\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n    scopes: 6\n  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n  sources:\n  - openapi/zocdoc-zocdoc-api-openapi.yml\n- name: AuthorizationCodeFlow\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n    scopes: 3\n  description: |-\n    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\n\
  \  sources:\n  - openapi/zocdoc-zocdoc-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/authentication/zocdoc-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Healthcare
- Appointments
- Booking
- Providers
- Insurance
- Telehealth
- Scheduling
---
