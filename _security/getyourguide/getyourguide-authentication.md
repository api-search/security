---
api_key_in:
- header
api_specs:
- filename: getyourguide-partner-openapi.yml
  format: yaml
  label: GetYourGuide Partner API
  slug: getyourguide-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getyourguide/refs/heads/main/openapi/getyourguide-partner-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Getyourguide Authentication
name_suffix: Authentication
oauth_flows: []
overview: GetYourGuide secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GetYourGuide
provider_slug: getyourguide
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-ACCESS-TOKEN
  sources:
  - openapi/getyourguide-partner-openapi.yml
  type: apiKey
slug: getyourguide-authentication
source_filename: getyourguide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/getyourguide-partner-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-ACCESS-TOKEN\n  sources:\n  - openapi/getyourguide-partner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getyourguide/refs/heads/main/authentication/getyourguide-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Travel
- Tourism
- Tours and Activities
- Marketplace
- Booking
- Experiences
- Affiliate
- Partner API
- Ecommerce
---
