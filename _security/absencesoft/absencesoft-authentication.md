---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Absencesoft Authentication
name_suffix: Authentication
oauth_flows:
- password
- clientCredentials
overview: AbsenceSoft secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and clientCredentials flow(s).
provider_name: AbsenceSoft
provider_slug: absencesoft
scheme_count: 1
schemes:
- description: The AbsenceSoft REST API uses OAuth2 for authorization, supporting both the resource-owner password credentials flow and the client credentials flow. All API communication is HTTPS-only across every endpoint.
  flows:
  - flow: password
  - flow: clientCredentials
  name: OAuth2
  sources:
  - docs
  type: oauth2
slug: absencesoft-authentication
source_filename: absencesoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://absencesoft.stoplight.io/docs/api-specs/46b38f624d360-welcome-to-the-absence-soft-api\ndocs: https://absencesoft.com/apis/\nsummary:\n  types: [oauth2]\n  oauth2_flows: [password, clientCredentials]\n  transport: https-only\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    The AbsenceSoft REST API uses OAuth2 for authorization, supporting both the\n    resource-owner password credentials flow and the client credentials flow.\n    All API communication is HTTPS-only across every endpoint.\n  flows:\n  - flow: password\n  - flow: clientCredentials\n  sources: [docs]\nnotes: >-\n  AbsenceSoft is API-first: the REST APIs available to customers are the same\n  ones that power the AbsenceSoft (AbsenceTracker) application itself. Token and\n  authorization endpoints are documented in the provider's Stoplight developer\n  portal behind customer login; scope names were not published on the public\n  surface and\
  \ are intentionally omitted here rather than fabricated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/absencesoft/refs/heads/main/authentication/absencesoft-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Leave Management
- Absence Management
- Accommodations
- HR Tech
- Compliance
- FMLA
- ADA
- Human Resources
---
