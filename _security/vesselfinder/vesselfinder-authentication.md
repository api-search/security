---
api_key_in:
- query
api_specs:
- filename: vesselfinder-ais-api-openapi.yml
  format: yaml
  label: VesselFinder AIS API
  slug: vesselfinder-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-ais-api-openapi.yml
- filename: vesselfinder-container-tracking-api-openapi.yml
  format: yaml
  label: VesselFinder Container Tracking API
  slug: vesselfinder-container-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-container-tracking-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vesselfinder Authentication
name_suffix: Authentication
oauth_flows: []
overview: VesselFinder secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VesselFinder
provider_slug: vesselfinder
scheme_count: 2
schemes:
- in: query
  name: UserKey
  parameter: userkey
  sources:
  - openapi/vesselfinder-ais-api-openapi.yml
  type: apiKey
- description: 'API key is passed as a path segment of the tracking URL, not as a header or query

    parameter. This security scheme is declarative only.'
  in: query
  name: PathApiKey
  parameter: apiKey
  sources:
  - openapi/vesselfinder-container-tracking-api-openapi.yml
  type: apiKey
slug: vesselfinder-authentication
source_filename: vesselfinder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vesselfinder-ais-api-openapi.yml, openapi/vesselfinder-container-tracking-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: UserKey\n  type: apiKey\n  in: query\n  parameter: userkey\n  sources:\n  - openapi/vesselfinder-ais-api-openapi.yml\n- name: PathApiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: |-\n    API key is passed as a path segment of the tracking URL, not as a header or query\n    parameter. This security scheme is declarative only.\n  sources:\n  - openapi/vesselfinder-container-tracking-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/authentication/vesselfinder-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- AIS
- Maritime
- Vessel Tracking
- Container Tracking
- Geospatial
- Logistics
- Ports
- Supply Chain
---
