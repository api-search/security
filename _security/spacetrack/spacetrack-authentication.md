---
api_key_in:
- cookie
api_specs:
- filename: spacetrack-ancillary-api-openapi.yml
  format: yaml
  label: Space-Track Ancillary API
  slug: spacetrack-ancillary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacetrack/refs/heads/main/openapi/spacetrack-ancillary-api-openapi.yml
- filename: spacetrack-authentication-api-openapi.yml
  format: yaml
  label: Space-Track Authentication API
  slug: spacetrack-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacetrack/refs/heads/main/openapi/spacetrack-authentication-api-openapi.yml
- filename: spacetrack-conjunction-data-api-openapi.yml
  format: yaml
  label: Space-Track Conjunction Data API
  slug: spacetrack-conjunction-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacetrack/refs/heads/main/openapi/spacetrack-conjunction-data-api-openapi.yml
- filename: spacetrack-decay-predictions-api-openapi.yml
  format: yaml
  label: Space-Track Decay Predictions API
  slug: spacetrack-decay-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacetrack/refs/heads/main/openapi/spacetrack-decay-predictions-api-openapi.yml
- filename: spacetrack-general-perturbations-api-openapi.yml
  format: yaml
  label: Space-Track General Perturbations API
  slug: spacetrack-general-perturbations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacetrack/refs/heads/main/openapi/spacetrack-general-perturbations-api-openapi.yml
- filename: spacetrack-satellite-catalog-api-openapi.yml
  format: yaml
  label: Space-Track Satellite Catalog API
  slug: spacetrack-satellite-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacetrack/refs/heads/main/openapi/spacetrack-satellite-catalog-api-openapi.yml
- filename: spacetrack-tracking-and-impact-prediction-api-openapi.yml
  format: yaml
  label: Space-Track Tracking and Impact Prediction API
  slug: spacetrack-tracking-and-impact-prediction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacetrack/refs/heads/main/openapi/spacetrack-tracking-and-impact-prediction-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spacetrack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Space-Track secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Space-Track
provider_slug: spacetrack
scheme_count: 1
schemes:
- description: Session cookie obtained by POSTing credentials to /ajaxauth/login
  in: cookie
  name: sessionCookie
  parameter: chocolatechip
  sources:
  - openapi/openapi.json
  type: apiKey
slug: spacetrack-authentication
source_filename: spacetrack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: chocolatechip\n  description: Session cookie obtained by POSTing credentials to /ajaxauth/login\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacetrack/refs/heads/main/authentication/spacetrack-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Space
- Satellites
- TLE
- Orbital Data
- Space Surveillance
- Debris Tracking
- Conjunction Data
- US Military
---
