---
api_key_in:
- header
api_specs:
- filename: docs
  format: yaml
  label: Pi-hole REST API
  slug: rest-api
  spec_type: OpenAPI
  url: http://pi.hole/api/docs
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pi Hole Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pi-hole secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pi-hole
provider_slug: pi-hole
scheme_count: 1
schemes:
- description: Session identifier returned by POST /api/auth.
  in: header
  name: sidHeader
  parameter: X-FTL-SID
  sources:
  - openapi/pi-hole-openapi.yml
  type: apiKey
slug: pi-hole-authentication
source_filename: pi-hole-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pi-hole-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sidHeader\n  type: apiKey\n  in: header\n  parameter: X-FTL-SID\n  description: Session identifier returned by POST /api/auth.\n  sources:\n  - openapi/pi-hole-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pi-hole/refs/heads/main/authentication/pi-hole-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DNS
- Ad Blocking
- Network Security
- Privacy
- Open Source
- Self-Hosted
---
