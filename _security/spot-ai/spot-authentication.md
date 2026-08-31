---
api_key_in: []
api_specs:
- filename: spot-ai-analytics-api-openapi.yml
  format: yaml
  label: Spot AI Analytics API
  slug: spot-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-analytics-api-openapi.yml
- filename: spot-ai-appliances-api-openapi.yml
  format: yaml
  label: Spot AI Appliances API
  slug: spot-ai-appliances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-appliances-api-openapi.yml
- filename: spot-ai-audio-api-openapi.yml
  format: yaml
  label: Spot AI Audio API
  slug: spot-ai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-audio-api-openapi.yml
- filename: spot-ai-cameras-api-openapi.yml
  format: yaml
  label: Spot AI Cameras API
  slug: spot-ai-cameras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-cameras-api-openapi.yml
- filename: spot-ai-embeds-api-openapi.yml
  format: yaml
  label: Spot AI Embeds API
  slug: spot-ai-embeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-embeds-api-openapi.yml
- filename: spot-ai-historical-footage-api-openapi.yml
  format: yaml
  label: Spot AI Historical Footage API
  slug: spot-ai-historical-footage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-historical-footage-api-openapi.yml
- filename: spot-ai-integration-devices-api-openapi.yml
  format: yaml
  label: Spot AI Integration Devices API
  slug: spot-ai-integration-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-integration-devices-api-openapi.yml
- filename: spot-ai-integration-event-types-api-openapi.yml
  format: yaml
  label: Spot AI Integration Event Types API
  slug: spot-ai-integration-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-integration-event-types-api-openapi.yml
- filename: spot-ai-integration-events-api-openapi.yml
  format: yaml
  label: Spot AI Integration Events API
  slug: spot-ai-integration-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-integration-events-api-openapi.yml
- filename: spot-ai-integrations-api-openapi.yml
  format: yaml
  label: Spot AI Integrations API
  slug: spot-ai-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-integrations-api-openapi.yml
- filename: spot-ai-locations-api-openapi.yml
  format: yaml
  label: Spot AI Locations API
  slug: spot-ai-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-locations-api-openapi.yml
- filename: spot-ai-lpi-api-openapi.yml
  format: yaml
  label: Spot AI LPI API
  slug: spot-ai-lpi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-lpi-api-openapi.yml
- filename: spot-ai-lpr-api-openapi.yml
  format: yaml
  label: Spot AI LPR API
  slug: spot-ai-lpr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-lpr-api-openapi.yml
- filename: spot-ai-shared-search-api-openapi.yml
  format: yaml
  label: Spot AI Shared Search API
  slug: spot-ai-shared-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-shared-search-api-openapi.yml
- filename: spot-ai-zones-api-openapi.yml
  format: yaml
  label: Spot AI Zones API
  slug: spot-ai-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/openapi/spot-ai-zones-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Spot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spot AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spot AI
provider_slug: spot-ai
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spot-ai/refs/heads/main/authentication/spot-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Video
- Physical Security
- Surveillance
- Computer-Vision
- Artificial Intelligence
- Camera
- Analytics
- License Plate Recognition
- Webhook
- Integration
---
