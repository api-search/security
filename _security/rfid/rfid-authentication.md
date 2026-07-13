---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rfid Authentication
name_suffix: Authentication
oauth_flows: []
overview: RFID secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RFID
provider_slug: rfid
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/rfid-epcis-openapi.yml
  type: http
slug: rfid-authentication
source_filename: rfid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rfid-epcis-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/rfid-epcis-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rfid/refs/heads/main/authentication/rfid-authentication.yml
summary_line: http · 1 scheme
tags:
- RFID
- IoT
- Supply Chain
- Inventory Management
- Asset Tracking
- GS1
- EPCIS
---
