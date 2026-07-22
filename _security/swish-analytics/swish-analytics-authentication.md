---
api_key_in:
- header
api_specs:
- filename: swish-analytics-sportsbook-openapi.yml
  format: yaml
  label: Swish Analytics Sportsbook API
  slug: swish-analytics-sportsbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swish-analytics/refs/heads/main/openapi/swish-analytics-sportsbook-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Swish Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swish Analytics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Swish Analytics
provider_slug: swish-analytics
scheme_count: 1
schemes:
- description: API key issued via the Swish Analytics developer portal (docs.swishanalytics.com). Managed under the /apikeys endpoints; passed in the ApiKey request header.
  in: header
  name: ApiKey
  parameter: ApiKey
  sources:
  - openapi/swish-analytics-sportsbook-openapi.yml
  type: apiKey
slug: swish-analytics-authentication
source_filename: swish-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/swish-analytics-sportsbook-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: ApiKey\n  description: API key issued via the Swish Analytics developer portal (docs.swishanalytics.com).\n    Managed under the /apikeys endpoints; passed in the ApiKey request header.\n  sources:\n  - openapi/swish-analytics-sportsbook-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swish-analytics/refs/heads/main/authentication/swish-analytics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Sports
- Sports Betting
- Sportsbook
- Analytics
- Machine Learning
- Odds
- Player Props
- Data
- Predictions
---
