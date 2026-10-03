---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bodyspec-api-status-api-openapi.yml
  format: yaml
  label: BodySpec API Status API
  slug: bodyspec-api-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-api-status-api-openapi.yml
- filename: bodyspec-appointments-api-openapi.yml
  format: yaml
  label: BodySpec Appointments API
  slug: bodyspec-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-appointments-api-openapi.yml
- filename: bodyspec-availability-api-openapi.yml
  format: yaml
  label: BodySpec Availability API
  slug: bodyspec-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-availability-api-openapi.yml
- filename: bodyspec-bodyspec-api-api-openapi.yml
  format: yaml
  label: BodySpec BodySpec API
  slug: bodyspec-bodyspec-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-bodyspec-api-api-openapi.yml
- filename: bodyspec-locations-api-openapi.yml
  format: yaml
  label: BodySpec Locations API
  slug: bodyspec-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-locations-api-openapi.yml
- filename: bodyspec-partner-appointments-api-openapi.yml
  format: yaml
  label: BodySpec Partner Appointments API
  slug: bodyspec-partner-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-appointments-api-openapi.yml
- filename: bodyspec-partner-intake-api-openapi.yml
  format: yaml
  label: BodySpec Partner Intake API
  slug: bodyspec-partner-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-intake-api-openapi.yml
- filename: bodyspec-partner-orders-api-openapi.yml
  format: yaml
  label: BodySpec Partner Orders API
  slug: bodyspec-partner-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-orders-api-openapi.yml
- filename: bodyspec-partner-results-api-openapi.yml
  format: yaml
  label: BodySpec Partner Results API
  slug: bodyspec-partner-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-results-api-openapi.yml
- filename: bodyspec-partner-users-api-openapi.yml
  format: yaml
  label: BodySpec Partner Users API
  slug: bodyspec-partner-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-users-api-openapi.yml
- filename: bodyspec-partner-webhooks-api-openapi.yml
  format: yaml
  label: BodySpec Partner Webhooks API
  slug: bodyspec-partner-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-webhooks-api-openapi.yml
- filename: bodyspec-reservations-api-openapi.yml
  format: yaml
  label: BodySpec Reservations API
  slug: bodyspec-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-reservations-api-openapi.yml
- filename: bodyspec-results-api-openapi.yml
  format: yaml
  label: BodySpec Results API
  slug: bodyspec-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-results-api-openapi.yml
- filename: bodyspec-services-api-openapi.yml
  format: yaml
  label: BodySpec Services API
  slug: bodyspec-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-services-api-openapi.yml
- filename: bodyspec-users-api-openapi.yml
  format: yaml
  label: BodySpec Users API
  slug: bodyspec-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-users-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Bodyspec Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BodySpec secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BodySpec
provider_slug: bodyspec
scheme_count: 3
schemes:
- description: OAuth2 authentication via Keycloak with PKCE
  flows:
  - authorizationUrl: https://auth.bodyspec.com/realms/bodyspec/protocol/openid-connect/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://auth.bodyspec.com/realms/bodyspec/protocol/openid-connect/token
  name: OAuth2
  sources:
  - openapi/bodyspec-openapi.json
  type: oauth2
- bearerFormat: JWT
  description: JWT Bearer token for authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/bodyspec-openapi.json
  type: http
- description: For partner integrations only. Contact BodySpec to obtain credentials.
  name: PartnerAuth
  scheme: basic
  sources:
  - openapi/bodyspec-openapi.json
  type: http
slug: bodyspec-authentication
source_filename: bodyspec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: derived\nsource: openapi/bodyspec-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.bodyspec.com/realms/bodyspec/protocol/openid-connect/auth\n    tokenUrl: https://auth.bodyspec.com/realms/bodyspec/protocol/openid-connect/token\n    scopes: 3\n  description: OAuth2 authentication via Keycloak with PKCE\n  sources:\n  - openapi/bodyspec-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT Bearer token for authentication\n  sources:\n  - openapi/bodyspec-openapi.json\n- name: PartnerAuth\n  type: http\n  scheme: basic\n  description: For partner integrations only. Contact BodySpec to obtain credentials.\n  sources:\n  - openapi/bodyspec-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/authentication/bodyspec-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Health
- Fitness
- API
- Data
---
