---
api_key_in:
- cookie
api_specs:
- filename: openapi.json
  format: json
  label: Space-Track API
  slug: space-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacetrack/refs/heads/main/openapi/openapi.json
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
