---
api_key_in: []
api_specs:
- filename: mx-platform-api-openapi.yml
  format: yaml
  label: MX Platform API
  slug: mx-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mx/refs/heads/main/openapi/mx-platform-api-openapi.yml
- filename: mx-consent-management-openapi.yml
  format: yaml
  label: MX Consent Management V4 API
  slug: mx-consent-management-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mx/refs/heads/main/openapi/mx-consent-management-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mx Authentication
name_suffix: Authentication
oauth_flows: []
overview: MX secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MX
provider_slug: mx
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mx-consent-management-openapi.yml
  - openapi/mx-platform-api-openapi.yml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/mx-consent-management-openapi.yml
  - openapi/mx-platform-api-openapi.yml
  type: http
slug: mx-authentication
source_filename: mx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/mx-consent-management-openapi.yml, openapi/mx-platform-api-openapi.yml\ndocs: https://docs.mx.com/resources/oauth-guide\nnotes: >-\n  MX Platform API authenticates with HTTP Basic auth over TLS: client_id is the\n  username and api_key is the password (Base64 in the Authorization header),\n  both issued from the Client Dashboard (dashboard.mx.com). The Consent\n  Management API additionally accepts a bearer token. OAuth in MX is an\n  institution-connection concern (Data Access / connecting members to their\n  banks), not an API-authorization scheme — there is no oauth2 securityScheme in\n  the API specs, so no OAuth scopes surface exists.\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/mx-consent-management-openapi.yml\n  - openapi/mx-platform-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/mx-consent-management-openapi.yml\n\
  \  - openapi/mx-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mx/refs/heads/main/authentication/mx-authentication.yml
summary_line: http · 2 schemes
tags:
- Financial-Services
- Banking
- United States
- Open Finance
- Data Aggregation
- FDX
- Fintech
- Financial Data
---
