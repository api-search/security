---
api_key_in: []
api_specs:
- filename: getaccept-archive-api-openapi.yml
  format: yaml
  label: GetAccept Archive API
  slug: getaccept-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-archive-api-openapi.yml
- filename: getaccept-attachments-api-openapi.yml
  format: yaml
  label: GetAccept Attachments API
  slug: getaccept-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-attachments-api-openapi.yml
- filename: getaccept-authentication-api-openapi.yml
  format: yaml
  label: GetAccept Authentication API
  slug: getaccept-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-authentication-api-openapi.yml
- filename: getaccept-communication-templates-api-openapi.yml
  format: yaml
  label: GetAccept Communication Templates API
  slug: getaccept-communication-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-communication-templates-api-openapi.yml
- filename: getaccept-contacts-api-openapi.yml
  format: yaml
  label: GetAccept Contacts API
  slug: getaccept-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-contacts-api-openapi.yml
- filename: getaccept-custom-data-api-openapi.yml
  format: yaml
  label: GetAccept Custom Data API
  slug: getaccept-custom-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-custom-data-api-openapi.yml
- filename: getaccept-documents-api-openapi.yml
  format: yaml
  label: GetAccept Documents API
  slug: getaccept-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-documents-api-openapi.yml
- filename: getaccept-others-api-openapi.yml
  format: yaml
  label: GetAccept Others API
  slug: getaccept-others-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-others-api-openapi.yml
- filename: getaccept-subscriptions-api-openapi.yml
  format: yaml
  label: GetAccept Subscriptions API
  slug: getaccept-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-subscriptions-api-openapi.yml
- filename: getaccept-templates-api-openapi.yml
  format: yaml
  label: GetAccept Templates API
  slug: getaccept-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-templates-api-openapi.yml
- filename: getaccept-users-api-openapi.yml
  format: yaml
  label: GetAccept Users API
  slug: getaccept-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-users-api-openapi.yml
- filename: getaccept-videos-api-openapi.yml
  format: yaml
  label: GetAccept Videos API
  slug: getaccept-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-videos-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Getaccept Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: GetAccept secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: GetAccept
provider_slug: getaccept
scheme_count: 2
schemes:
- description: For testing purpose, use client_id **api** and client_secret **app**
  flows:
  - authorizationUrl: https://app.getaccept.com/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://app.getaccept.com/oauth2/token
  name: Oauth2
  sources:
  - openapi/getaccept-openapi-original.json
  type: oauth2
- bearerFormat: JWT
  description: Enter your bearer token
  name: Token
  scheme: bearer
  sources:
  - openapi/getaccept-openapi-original.json
  type: http
slug: getaccept-authentication
source_filename: getaccept-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/getaccept-openapi-original.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: Oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.getaccept.com/oauth2/authorize\n    tokenUrl: https://app.getaccept.com/oauth2/token\n    scopes: 1\n  description: For testing purpose, use client_id **api** and client_secret **app**\n  sources:\n  - openapi/getaccept-openapi-original.json\n- name: Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter your bearer token\n  sources:\n  - openapi/getaccept-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/authentication/getaccept-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Cloud
- Sales Enablement
- Electronic Signature
- E-Signature
- Digital Sales Room
- Document Management
- Contract Management
- Proposals
- SaaS
---
