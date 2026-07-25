---
api_key_in:
- header
api_specs:
- filename: encharge-account-api-openapi.yml
  format: yaml
  label: Encharge Account API
  slug: encharge-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-account-api-openapi.yml
- filename: encharge-events-api-openapi.yml
  format: yaml
  label: Encharge Events API
  slug: encharge-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-events-api-openapi.yml
- filename: encharge-fields-api-openapi.yml
  format: yaml
  label: Encharge Fields API
  slug: encharge-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-fields-api-openapi.yml
- filename: encharge-ingest-api-openapi.yml
  format: yaml
  label: Encharge Ingest API
  slug: encharge-ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-ingest-api-openapi.yml
- filename: encharge-people-api-openapi.yml
  format: yaml
  label: Encharge People API
  slug: encharge-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-people-api-openapi.yml
- filename: encharge-segments-api-openapi.yml
  format: yaml
  label: Encharge Segments API
  slug: encharge-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-segments-api-openapi.yml
- filename: encharge-tags-api-openapi.yml
  format: yaml
  label: Encharge Tags API
  slug: encharge-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-tags-api-openapi.yml
- filename: encharge-transactional-email-api-openapi.yml
  format: yaml
  label: Encharge Transactional Email API
  slug: encharge-transactional-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-transactional-email-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Encharge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Encharge secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Encharge
provider_slug: encharge
scheme_count: 2
schemes:
- in: header
  name: tokenHeader
  parameter: X-Encharge-Token
  sources:
  - openapi/encharge-openapi.yml
  type: apiKey
- name: bearer
  scheme: bearer
  sources:
  - openapi/encharge-openapi.yml
  type: http
slug: encharge-authentication
source_filename: encharge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/encharge-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: tokenHeader\n  type: apiKey\n  in: header\n  parameter: X-Encharge-Token\n  sources:\n  - openapi/encharge-openapi.yml\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/encharge-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/authentication/encharge-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Email Marketing
- Marketing Automation
- Transactional Email
- SaaS
- Behavioral Email
- Customer Engagement
---
