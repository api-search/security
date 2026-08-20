---
api_key_in: []
api_specs:
- filename: hopin-bank-questions-api-openapi.yml
  format: yaml
  label: RingCentral Events Bank Questions API
  slug: hopin-bank-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-bank-questions-api-openapi.yml
- filename: hopin-booths-api-openapi.yml
  format: yaml
  label: RingCentral Events Booths API
  slug: hopin-booths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-booths-api-openapi.yml
- filename: hopin-data-subscriptions-api-openapi.yml
  format: yaml
  label: RingCentral Events Data Subscriptions API
  slug: hopin-data-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-data-subscriptions-api-openapi.yml
- filename: hopin-events-api-openapi.yml
  format: yaml
  label: RingCentral Events Events API
  slug: hopin-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-events-api-openapi.yml
- filename: hopin-health-api-openapi.yml
  format: yaml
  label: RingCentral Events Health API
  slug: hopin-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-health-api-openapi.yml
- filename: hopin-magic-links-api-openapi.yml
  format: yaml
  label: RingCentral Events Magic Links API
  slug: hopin-magic-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-magic-links-api-openapi.yml
- filename: hopin-organizations-api-openapi.yml
  format: yaml
  label: RingCentral Events Organizations API
  slug: hopin-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-organizations-api-openapi.yml
- filename: hopin-registrations-api-openapi.yml
  format: yaml
  label: RingCentral Events Registrations API
  slug: hopin-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-registrations-api-openapi.yml
- filename: hopin-reports-api-openapi.yml
  format: yaml
  label: RingCentral Events Reports API
  slug: hopin-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-reports-api-openapi.yml
- filename: hopin-schedule-items-api-openapi.yml
  format: yaml
  label: RingCentral Events Schedule Items API
  slug: hopin-schedule-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-schedule-items-api-openapi.yml
- filename: hopin-sessions-api-openapi.yml
  format: yaml
  label: RingCentral Events Sessions API
  slug: hopin-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-sessions-api-openapi.yml
- filename: hopin-stages-api-openapi.yml
  format: yaml
  label: RingCentral Events Stages API
  slug: hopin-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-stages-api-openapi.yml
- filename: hopin-templates-api-openapi.yml
  format: yaml
  label: RingCentral Events Templates API
  slug: hopin-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-templates-api-openapi.yml
- filename: hopin-tickets-api-openapi.yml
  format: yaml
  label: RingCentral Events Tickets API
  slug: hopin-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-tickets-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hopin Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: RingCentral Events secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: RingCentral Events
provider_slug: hopin
scheme_count: 1
schemes:
- description: OAuth 2.0 Client Credentials flow
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.events.ringcentral.com/v1/auth/token
  name: oauth2
  sources:
  - openapi/openapi.json
  type: oauth2
slug: hopin-authentication
source_filename: hopin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.events.ringcentral.com/v1/auth/token\n    scopes: 2\n  description: OAuth 2.0 Client Credentials flow\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/authentication/hopin-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Event
- Virtual Events
- Hybrid Events
- Webinars
- Event Management
- Registration
- Sessions
- Networking
---
