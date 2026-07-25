---
api_key_in: []
api_specs:
- filename: spot-analytics-api-openapi.yml
  format: yaml
  label: Spot Analytics API
  slug: spot-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-analytics-api-openapi.yml
- filename: spot-appliances-api-openapi.yml
  format: yaml
  label: Spot Appliances API
  slug: spot-appliances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-appliances-api-openapi.yml
- filename: spot-audio-api-openapi.yml
  format: yaml
  label: Spot Audio API
  slug: spot-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-audio-api-openapi.yml
- filename: spot-cameras-api-openapi.yml
  format: yaml
  label: Spot Cameras API
  slug: spot-cameras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-cameras-api-openapi.yml
- filename: spot-embeds-api-openapi.yml
  format: yaml
  label: Spot Embeds API
  slug: spot-embeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-embeds-api-openapi.yml
- filename: spot-historical-footage-api-openapi.yml
  format: yaml
  label: Spot Historical Footage API
  slug: spot-historical-footage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-historical-footage-api-openapi.yml
- filename: spot-integration-devices-api-openapi.yml
  format: yaml
  label: Spot Integration Devices API
  slug: spot-integration-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-integration-devices-api-openapi.yml
- filename: spot-integration-event-types-api-openapi.yml
  format: yaml
  label: Spot Integration Event Types API
  slug: spot-integration-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-integration-event-types-api-openapi.yml
- filename: spot-integration-events-api-openapi.yml
  format: yaml
  label: Spot Integration Events API
  slug: spot-integration-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-integration-events-api-openapi.yml
- filename: spot-integrations-api-openapi.yml
  format: yaml
  label: Spot Integrations API
  slug: spot-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-integrations-api-openapi.yml
- filename: spot-locations-api-openapi.yml
  format: yaml
  label: Spot Locations API
  slug: spot-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-locations-api-openapi.yml
- filename: spot-lpi-api-openapi.yml
  format: yaml
  label: Spot LPI API
  slug: spot-lpi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-lpi-api-openapi.yml
- filename: spot-lpr-api-openapi.yml
  format: yaml
  label: Spot LPR API
  slug: spot-lpr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-lpr-api-openapi.yml
- filename: spot-shared-search-api-openapi.yml
  format: yaml
  label: Spot Shared Search API
  slug: spot-shared-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-shared-search-api-openapi.yml
- filename: spot-zones-api-openapi.yml
  format: yaml
  label: Spot Zones API
  slug: spot-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/openapi/spot-zones-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Spot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spot secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spot
provider_slug: spot
scheme_count: 1
schemes:
- name: bearer_security
  scheme: bearer
  sources:
  - openapi/spot-connect-openapi.json
  - openapi/spot-devices-openapi.json
  - openapi/spot-intelligence-openapi.json
  type: http
slug: spot-authentication
source_filename: spot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/spot-connect-openapi.json, openapi/spot-devices-openapi.json, openapi/spot-intelligence-openapi.json\ndocs: https://developers.spot.ai/reference/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\nnotes: >-\n  Spot AI uses a bearer API key. An organization admin generates an API key on\n  the API settings page of the Spot dashboard (Create New Key -> name it ->\n  optional expiration, defaults to 1 year -> Generate Key). The key is shown\n  only once at creation. Keys are authorized by role (Owner recommended for full\n  access) with an optional resource scope. The key is sent as an HTTP bearer\n  token. Individual operations further require named permissions (e.g.\n  camera_share_create, clip_share_create, camera.manage_audio).\nschemes:\n- name: bearer_security\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/spot-connect-openapi.json\n  - openapi/spot-devices-openapi.json\n  - openapi/spot-intelligence-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/authentication/spot-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Video
- Physical Security
- Surveillance
- Computer Vision
- Artificial Intelligence
- Cameras
- Analytics
- License Plate Recognition
- Webhooks
- Integrations
---
