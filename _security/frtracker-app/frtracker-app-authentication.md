---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Federal Regulatory Tracker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Federal Regulatory Tracker secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Federal Regulatory Tracker
provider_slug: frtracker-app
scheme_count: 1
schemes:
- description: Required for most endpoints, including general search, Provision History search, and all data exports. Health, timeliness, stats, changes, weekly-summary, the bounded H-2A provenance example, Provision History dossier detail, and per-document comments are keyless.
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/frtracker-app-openapi.yml
  type: apiKey
slug: frtracker-app-authentication
source_filename: frtracker-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/frtracker-app-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Required for most endpoints, including general search, Provision History search,\n    and all data exports. Health, timeliness, stats, changes, weekly-summary, the bounded H-2A\n    provenance example, Provision History dossier detail, and per-document comments are keyless.\n  sources:\n  - openapi/frtracker-app-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/frtracker-app/authentication/frtracker-app-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Regulatory Research
- Data Services
- Federal Register
---
