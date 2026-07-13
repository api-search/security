---
api_key_in:
- header
api_specs:
- filename: visio-javascript-openapi.yml
  format: yaml
  label: Visio JavaScript API
  slug: visio-javascript-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visio/refs/heads/main/openapi/visio-javascript-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Visio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Visio API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Visio API
provider_slug: visio
scheme_count: 1
schemes:
- description: Visio EmbeddedSession token obtained via OfficeExtension.EmbeddedSession initialization
  in: header
  name: EmbeddedSession
  parameter: X-Embedded-Session
  sources:
  - openapi/visio-javascript-openapi.yml
  type: apiKey
slug: visio-authentication
source_filename: visio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/visio-javascript-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: EmbeddedSession\n  type: apiKey\n  in: header\n  parameter: X-Embedded-Session\n  description: Visio EmbeddedSession token obtained via OfficeExtension.EmbeddedSession initialization\n  sources:\n  - openapi/visio-javascript-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visio/refs/heads/main/authentication/visio-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Business Process
- Collaboration
- Diagrams
- Enterprise
- Flowcharts
- Microsoft 365
- Visualization
---
