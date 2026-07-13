---
api_key_in: []
api_specs:
- filename: OpenAPI_3_0
  format: yaml
  label: Boomi Platform REST API
  slug: platform-rest-api
  spec_type: OpenAPI
  url: https://developer.boomi.com/docs/APIs/PlatformAPI/Introduction/OpenAPI_3_0
- filename: OpenAPI_3_0
  format: yaml
  label: Boomi Platform Partner API
  slug: platform-partner-api
  spec_type: OpenAPI
  url: https://developer.boomi.com/docs/APIs/PlatformAPI/Introduction/OpenAPI_3_0
- filename: boomi-datahub-api-openapi.yml
  format: yaml
  label: Boomi DataHub API
  slug: datahub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-datahub-api-openapi.yml
- filename: boomi-event-streams-openapi.yml
  format: yaml
  label: Boomi Event Streams REST API
  slug: event-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-event-streams-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Boomi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boomi secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Boomi
provider_slug: boomi
scheme_count: 2
schemes:
- description: Basic Authentication for the DataHub Platform API. Users with two-factor authentication must include an X-Boomi-OTP header.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/boomi-datahub-api-openapi.yml
  - openapi/boomi-platform-rest-api-openapi.yml
  type: http
- description: JWT Bearer token for the Repository API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/boomi-datahub-api-openapi.yml
  - openapi/boomi-event-streams-openapi.yml
  type: http
slug: boomi-authentication
source_filename: boomi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/boomi-datahub-api-openapi.yml, openapi/boomi-event-streams-openapi.yml, openapi/boomi-platform-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic Authentication for the DataHub Platform API. Users with two-factor authentication\n    must include an X-Boomi-OTP header.\n  sources:\n  - openapi/boomi-datahub-api-openapi.yml\n  - openapi/boomi-platform-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: JWT Bearer token for the Repository API.\n  sources:\n  - openapi/boomi-datahub-api-openapi.yml\n  - openapi/boomi-event-streams-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/authentication/boomi-authentication.yml
summary_line: http · 2 schemes
tags:
- AI Agents
- Automation
- B2B
- Data Integration
- EDI
- Integrations
- Management
- MFT
- Platform
- Workflows
---
