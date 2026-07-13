---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: TIBCO Cloud Integration API
  slug: tibco-cloud-integration-api
  spec_type: OpenAPI
  url: https://integration.cloud.tibco.com/docs/api/openapi.json
- filename: io-docs
  format: yaml
  label: TIBCO Mashery API Management
  slug: tibco-mashery-api-management
  spec_type: OpenAPI
  url: https://developer.mashery.com/io-docs
- filename: tibco-businessevents-openapi.yml
  format: yaml
  label: TIBCO BusinessEvents API
  slug: tibco-businessevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tibco/refs/heads/main/openapi/tibco-businessevents-openapi.yml
- filename: tibco-messaging-asyncapi.yml
  format: yaml
  label: TIBCO Messaging API
  slug: tibco-messaging-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tibco/refs/heads/main/asyncapi/tibco-messaging-asyncapi.yml
- filename: tibco-spotfire-openapi.yml
  format: yaml
  label: TIBCO Spotfire Analytics API
  slug: tibco-spotfire-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tibco/refs/heads/main/openapi/tibco-spotfire-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tibco Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: TIBCO secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: TIBCO
provider_slug: tibco
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token for TIBCO BusinessEvents API access
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tibco-businessevents-openapi.yml
  - openapi/tibco-cloud-integration-openapi.yml
  - openapi/tibco-spotfire-openapi.yml
  type: http
- description: OAuth 2.0 client credentials for Mashery API access
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.mashery.com/v3/token
  name: oauth2
  sources:
  - openapi/tibco-mashery-openapi.yml
  type: oauth2
- description: Basic authentication for on-premise Spotfire Server
  name: basicAuth
  scheme: basic
  sources:
  - openapi/tibco-spotfire-openapi.yml
  type: http
slug: tibco-authentication
source_filename: tibco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tibco-businessevents-openapi.yml, openapi/tibco-cloud-integration-openapi.yml,\n  openapi/tibco-mashery-openapi.yml, openapi/tibco-spotfire-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token for TIBCO BusinessEvents API access\n  sources:\n  - openapi/tibco-businessevents-openapi.yml\n  - openapi/tibco-cloud-integration-openapi.yml\n  - openapi/tibco-spotfire-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.mashery.com/v3/token\n    scopes: 0\n  description: OAuth 2.0 client credentials for Mashery API access\n  sources:\n  - openapi/tibco-mashery-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication for on-premise Spotfire Server\n  sources:\n  - openapi/tibco-spotfire-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tibco/refs/heads/main/authentication/tibco-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Analytics
- API Management
- Cloud
- Enterprise Software
- Integration
- Messaging
- Real-Time Data
---
