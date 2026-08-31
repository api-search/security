---
api_key_in:
- query
api_specs:
- filename: airlabs-airlines-api-openapi.yml
  format: yaml
  label: Airlabs Airlines API
  slug: airlabs-airlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-airlines-api-openapi.yml
- filename: airlabs-airports-api-openapi.yml
  format: yaml
  label: Airlabs Airports API
  slug: airlabs-airports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-airports-api-openapi.yml
- filename: airlabs-alert-api-openapi.yml
  format: yaml
  label: Airlabs Alert API
  slug: airlabs-alert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-alert-api-openapi.yml
- filename: airlabs-cities-api-openapi.yml
  format: yaml
  label: Airlabs Cities API
  slug: airlabs-cities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-cities-api-openapi.yml
- filename: airlabs-delays-api-openapi.yml
  format: yaml
  label: Airlabs Delays API
  slug: airlabs-delays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-delays-api-openapi.yml
- filename: airlabs-fleets-api-openapi.yml
  format: yaml
  label: Airlabs Fleets API
  slug: airlabs-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-fleets-api-openapi.yml
- filename: airlabs-flight-api-openapi.yml
  format: yaml
  label: Airlabs Flight API
  slug: airlabs-flight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-flight-api-openapi.yml
- filename: airlabs-flights-api-openapi.yml
  format: yaml
  label: Airlabs Flights API
  slug: airlabs-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-flights-api-openapi.yml
- filename: airlabs-nearby-api-openapi.yml
  format: yaml
  label: Airlabs Nearby API
  slug: airlabs-nearby-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-nearby-api-openapi.yml
- filename: airlabs-routes-api-openapi.yml
  format: yaml
  label: Airlabs Routes API
  slug: airlabs-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-routes-api-openapi.yml
- filename: airlabs-schedules-api-openapi.yml
  format: yaml
  label: Airlabs Schedules API
  slug: airlabs-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-schedules-api-openapi.yml
- filename: airlabs-suggest-api-openapi.yml
  format: yaml
  label: Airlabs Suggest API
  slug: airlabs-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-suggest-api-openapi.yml
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
