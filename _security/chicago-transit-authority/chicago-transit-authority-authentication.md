---
api_key_in:
- query
api_specs:
- filename: chicago-transit-authority-arrivals-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Arrivals API
  slug: chicago-transit-authority-arrivals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-arrivals-api-openapi.yml
- filename: chicago-transit-authority-bulletins-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Bulletins API
  slug: chicago-transit-authority-bulletins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-bulletins-api-openapi.yml
- filename: chicago-transit-authority-follow-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Follow API
  slug: chicago-transit-authority-follow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-follow-api-openapi.yml
- filename: chicago-transit-authority-locations-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Locations API
  slug: chicago-transit-authority-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-locations-api-openapi.yml
- filename: chicago-transit-authority-predictions-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Predictions API
  slug: chicago-transit-authority-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-predictions-api-openapi.yml
- filename: chicago-transit-authority-routes-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Routes API
  slug: chicago-transit-authority-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-routes-api-openapi.yml
- filename: chicago-transit-authority-stops-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Stops API
  slug: chicago-transit-authority-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-stops-api-openapi.yml
- filename: chicago-transit-authority-system-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority System API
  slug: chicago-transit-authority-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-system-api-openapi.yml
- filename: chicago-transit-authority-vehicles-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Vehicles API
  slug: chicago-transit-authority-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-vehicles-api-openapi.yml
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
