---
api_key_in:
- query
api_specs:
- filename: cta-train-tracker-openapi.yml
  format: yaml
  label: CTA Train Tracker API
  slug: train-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/cta-train-tracker-openapi.yml
- filename: cta-bus-tracker-openapi.yml
  format: yaml
  label: CTA Bus Tracker API
  slug: bus-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/cta-bus-tracker-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Chicago Transit Authority Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chicago Transit Authority secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chicago Transit Authority
provider_slug: chicago-transit-authority
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/cta-bus-tracker-openapi.yml
  - openapi/cta-train-tracker-openapi.yml
  type: apiKey
slug: chicago-transit-authority-authentication
source_filename: chicago-transit-authority-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cta-bus-tracker-openapi.yml, openapi/cta-train-tracker-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/cta-bus-tracker-openapi.yml\n  - openapi/cta-train-tracker-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/authentication/chicago-transit-authority-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bus
- Bus Tracker
- Chicago
- CTA
- Customer Alerts
- GTFS
- L Train
- Open Data
- Public Transit
- Real-Time
- Train
- Train Tracker
- Transit
- Transportation
---
