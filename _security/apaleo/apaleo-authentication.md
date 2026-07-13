---
api_key_in: []
api_specs:
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Booking API
  slug: booking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Inventory API
  slug: inventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Rate Plan API
  slug: rateplan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Availability API
  slug: availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Finance API
  slug: finance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Settings API
  slug: settings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Webhook API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Apaleo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: apaleo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: apaleo
provider_slug: apaleo
scheme_count: 1
schemes:
- description: apaleo uses OAuth 2.0. Obtain a bearer access token from the apaleo identity provider and send it in the Authorization header as 'Bearer {token}'. The client-credentials and authorization-code grants are supported.
  flows:
  - flow: clientCredentials
    scopes: 10
    tokenUrl: https://identity.apaleo.com/connect/token
  - authorizationUrl: https://identity.apaleo.com/connect/authorize
    flow: authorizationCode
    scopes: 10
    tokenUrl: https://identity.apaleo.com/connect/token
  name: oauth2
  sources:
  - openapi/apaleo-openapi.yml
  type: oauth2
slug: apaleo-authentication
source_filename: apaleo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apaleo-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.apaleo.com/connect/token\n    scopes: 10\n  - flow: authorizationCode\n    authorizationUrl: https://identity.apaleo.com/connect/authorize\n    tokenUrl: https://identity.apaleo.com/connect/token\n    scopes: 10\n  description: apaleo uses OAuth 2.0. Obtain a bearer access token from the apaleo identity\n    provider and send it in the Authorization header as 'Bearer {token}'. The client-credentials\n    and authorization-code grants are supported.\n  sources:\n  - openapi/apaleo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/authentication/apaleo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Hospitality
- PMS
- Property Management
- Hotels
- API-First
---
