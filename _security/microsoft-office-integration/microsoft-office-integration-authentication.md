---
api_key_in: []
api_specs:
- filename: microsoft-office-management-activity-api-openapi.yml
  format: yaml
  label: Microsoft Office 365 Management Activity API
  slug: management-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/openapi/microsoft-office-management-activity-api-openapi.yml
- filename: microsoft-office-service-communications-api-openapi.yml
  format: yaml
  label: Microsoft Office 365 Service Communications API
  slug: service-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/openapi/microsoft-office-service-communications-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Office Integration Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Office Integration secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Office Integration
provider_slug: microsoft-office-integration
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth2 JWT access token obtained from Microsoft Entra ID with ActivityFeed.Read claim.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-office-management-activity-api-openapi.yml
  - openapi/microsoft-office-service-communications-api-openapi.yml
  type: http
slug: microsoft-office-integration-authentication
source_filename: microsoft-office-integration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-office-management-activity-api-openapi.yml, openapi/microsoft-office-service-communications-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 JWT access token obtained from Microsoft Entra ID with ActivityFeed.Read\n    claim.\n  sources:\n  - openapi/microsoft-office-management-activity-api-openapi.yml\n  - openapi/microsoft-office-service-communications-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/authentication/microsoft-office-integration-authentication.yml
summary_line: http · 1 scheme
tags:
- Microsoft 365
- Microsoft Office Integration
- Office 365
---
