---
api_key_in:
- query
api_specs:
- filename: vesselfinder-containers-api-openapi.yml
  format: yaml
  label: VesselFinder Containers API
  slug: vesselfinder-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-containers-api-openapi.yml
- filename: vesselfinder-distance-api-openapi.yml
  format: yaml
  label: VesselFinder Distance API
  slug: vesselfinder-distance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-distance-api-openapi.yml
- filename: vesselfinder-expected-arrivals-api-openapi.yml
  format: yaml
  label: VesselFinder Expected Arrivals API
  slug: vesselfinder-expected-arrivals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-expected-arrivals-api-openapi.yml
- filename: vesselfinder-list-manager-api-openapi.yml
  format: yaml
  label: VesselFinder List Manager API
  slug: vesselfinder-list-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-list-manager-api-openapi.yml
- filename: vesselfinder-live-data-api-openapi.yml
  format: yaml
  label: VesselFinder Live Data API
  slug: vesselfinder-live-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-live-data-api-openapi.yml
- filename: vesselfinder-master-data-api-openapi.yml
  format: yaml
  label: VesselFinder Master Data API
  slug: vesselfinder-master-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-master-data-api-openapi.yml
- filename: vesselfinder-port-calls-api-openapi.yml
  format: yaml
  label: VesselFinder Port Calls API
  slug: vesselfinder-port-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-port-calls-api-openapi.yml
- filename: vesselfinder-status-api-openapi.yml
  format: yaml
  label: VesselFinder Status API
  slug: vesselfinder-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-status-api-openapi.yml
- filename: vesselfinder-vessels-api-openapi.yml
  format: yaml
  label: VesselFinder Vessels API
  slug: vesselfinder-vessels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-vessels-api-openapi.yml
- filename: vesselfinder-vessels-list-api-openapi.yml
  format: yaml
  label: VesselFinder Vessels List API
  slug: vesselfinder-vessels-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-vessels-list-api-openapi.yml
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
