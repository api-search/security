---
api_key_in: []
api_specs:
- filename: windstream-voice-openapi.yml
  format: yaml
  label: Windstream Enterprise Voice API
  slug: windstream-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-voice-openapi.yml
- filename: windstream-contact-center-openapi.yml
  format: yaml
  label: Windstream Enterprise Contact Center Services API
  slug: windstream-contact-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-contact-center-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Windstream Holdings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Windstream Holdings secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Windstream Holdings
provider_slug: windstream-holdings
scheme_count: 2
schemes:
- description: Bearer token authentication for CCS API
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/windstream-contact-center-openapi.yml
  type: http
- description: 'HTTP Basic Authentication using extension@tenantId credentials. Username formats: ext@tenantId, ext@tenantId.ID, ext@tenantDID.DID, ext@tenantURI.URI'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/windstream-voice-openapi.yml
  type: http
slug: windstream-holdings-authentication
source_filename: windstream-holdings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/windstream-contact-center-openapi.yml, openapi/windstream-voice-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication for CCS API\n  sources:\n  - openapi/windstream-contact-center-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic Authentication using extension@tenantId credentials. Username formats:\n    ext@tenantId, ext@tenantId.ID, ext@tenantDID.DID, ext@tenantURI.URI'\n  sources:\n  - openapi/windstream-voice-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/authentication/windstream-holdings-authentication.yml
summary_line: http · 2 schemes
tags:
- Broadband
- Contact Center
- Managed Services
- Network Communications
- SD-WAN
- Telecom
- UCaaS
- Unified Communications
- Fortune 500
---
