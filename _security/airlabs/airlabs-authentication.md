---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Airlabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airlabs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Airlabs
provider_slug: airlabs
scheme_count: 1
schemes:
- description: API key. Sign up at https://airlabs.co/signup
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/openapi.yaml
  type: apiKey
slug: airlabs-authentication
source_filename: airlabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key. Sign up at https://airlabs.co/signup\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/authentication/airlabs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Aviation
- Flights
- Airlines
- Airports
- Flight Tracking
- Flight Status
- Real-time Data
---
