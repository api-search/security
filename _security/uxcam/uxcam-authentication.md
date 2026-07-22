---
api_key_in:
- header
api_specs:
- filename: uxcam-data-access-openapi.yml
  format: yaml
  label: UXCam Data Access API
  slug: uxcam-data-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uxcam/refs/heads/main/openapi/uxcam-data-access-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Uxcam Authentication
name_suffix: Authentication
oauth_flows: []
overview: UXCam secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: UXCam
provider_slug: uxcam
scheme_count: 2
schemes:
- description: Identifier for the app created in the UXCam Dashboard; required on every Data Access API request.
  in: header
  name: AppId
  parameter: X-App-Id
  type: apiKey
- description: Randomly generated authentication key issued from the UXCam Dashboard; validates UXCam Data Access API requests only.
  in: header
  name: ApiKey
  parameter: X-Api-Key
  type: apiKey
slug: uxcam-authentication
source_filename: uxcam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://developer.uxcam.com/docs/data-access-api\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\nschemes:\n  - name: AppId\n    type: apiKey\n    in: header\n    parameter: X-App-Id\n    description: Identifier for the app created in the UXCam Dashboard; required on\n      every Data Access API request.\n  - name: ApiKey\n    type: apiKey\n    in: header\n    parameter: X-Api-Key\n    description: Randomly generated authentication key issued from the UXCam\n      Dashboard; validates UXCam Data Access API requests only.\nnotes: The Data Access API (https://api.uxcam.com/v2) authenticates with the\n  X-App-Id + X-Api-Key header pair. The mobile/web SDKs are configured with a\n  separate app key at SDK initialization; no OAuth surface is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uxcam/refs/heads/main/authentication/uxcam-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Product Analytics
- Session Replay
- Mobile Analytics
- Heatmaps
- User Experience
- Crash Reporting
---
