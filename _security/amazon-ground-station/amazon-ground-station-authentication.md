---
api_key_in:
- header
api_specs:
- filename: amazon-ground-station-agent-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Agent API
  slug: amazon-ground-station-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-agent-api-openapi.yml
- filename: amazon-ground-station-config-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Config API
  slug: amazon-ground-station-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-config-api-openapi.yml
- filename: amazon-ground-station-contact-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Contact API
  slug: amazon-ground-station-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-contact-api-openapi.yml
- filename: amazon-ground-station-contacts-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Contacts API
  slug: amazon-ground-station-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-contacts-api-openapi.yml
- filename: amazon-ground-station-dataflowendpointgroup-api-openapi.yml
  format: yaml
  label: Amazon Ground Station DataflowEndpointGroup API
  slug: amazon-ground-station-dataflowendpointgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-dataflowendpointgroup-api-openapi.yml
- filename: amazon-ground-station-ephemerides-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Ephemerides API
  slug: amazon-ground-station-ephemerides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-ephemerides-api-openapi.yml
- filename: amazon-ground-station-ephemeris-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Ephemeris API
  slug: amazon-ground-station-ephemeris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-ephemeris-api-openapi.yml
- filename: amazon-ground-station-groundstation-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Groundstation API
  slug: amazon-ground-station-groundstation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-groundstation-api-openapi.yml
- filename: amazon-ground-station-minute-usage-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Minute Usage API
  slug: amazon-ground-station-minute-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-minute-usage-api-openapi.yml
- filename: amazon-ground-station-missionprofile-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Missionprofile API
  slug: amazon-ground-station-missionprofile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-missionprofile-api-openapi.yml
- filename: amazon-ground-station-satellite-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Satellite API
  slug: amazon-ground-station-satellite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-satellite-api-openapi.yml
- filename: amazon-ground-station-tags-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Tags API
  slug: amazon-ground-station-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Ground Station Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Ground Station secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-ground-station-openapi.yaml
  type: apiKey
slug: amazon-ground-station-authentication
source_filename: amazon-ground-station-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-ground-station-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-ground-station-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/authentication/amazon-ground-station-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
---
