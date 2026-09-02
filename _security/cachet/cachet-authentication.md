---
api_key_in:
- header
api_specs:
- filename: cachet-connect-api-openapi.yml
  format: yaml
  label: Cachet Connect API
  slug: cachet-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cachet/refs/heads/main/openapi/cachet-connect-api-openapi.yml
- filename: cachet-gig-events-api-openapi.yml
  format: yaml
  label: Cachet Gig-Events API
  slug: cachet-gig-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cachet/refs/heads/main/openapi/cachet-gig-events-api-openapi.yml
- filename: cachet-user-api-openapi.yml
  format: yaml
  label: Cachet User API
  slug: cachet-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cachet/refs/heads/main/openapi/cachet-user-api-openapi.yml
- filename: cachet-vehicle-events-api-openapi.yml
  format: yaml
  label: Cachet Vehicle events API
  slug: cachet-vehicle-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cachet/refs/heads/main/openapi/cachet-vehicle-events-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cachet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cachet secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cachet
provider_slug: cachet
scheme_count: 2
schemes:
- description: Username provided by Cachet IT
  in: header
  name: x-api-username
  parameter: x-api-username
  sources:
  - openapi/cachet-parking-openapi.yml
  - openapi/cachet-partners-openapi.yml
  - openapi/cachet-verify-openapi.yml
  type: apiKey
- description: API Key provided by Cachet IT
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/cachet-parking-openapi.yml
  - openapi/cachet-partners-openapi.yml
  - openapi/cachet-verify-openapi.yml
  type: apiKey
slug: cachet-authentication
source_filename: cachet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cachet-parking-openapi.yml, openapi/cachet-partners-openapi.yml, openapi/cachet-verify-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x-api-username\n  type: apiKey\n  in: header\n  parameter: x-api-username\n  description: Username provided by Cachet IT\n  sources:\n  - openapi/cachet-parking-openapi.yml\n  - openapi/cachet-partners-openapi.yml\n  - openapi/cachet-verify-openapi.yml\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API Key provided by Cachet IT\n  sources:\n  - openapi/cachet-parking-openapi.yml\n  - openapi/cachet-partners-openapi.yml\n  - openapi/cachet-verify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cachet/refs/heads/main/authentication/cachet-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Insurance
- Insurtech
- Mobility
- Gig Economy
- Car Sharing
- Embedded Insurance
- Event
---
