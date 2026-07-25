---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Pointonenav Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pointonenav declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Pointonenav
provider_slug: pointonenav
scheme_count: 2
schemes:
- api: Point One GraphQL API
  description: API-key authenticated GraphQL endpoint for workflow and data management.
  docs: https://docs.pointonenav.com/docs/graphql-api/quickstart
  in: header
  key_source: https://app.pointonenav.com
  type: apiKey
- api: Polaris RTK Network Service
  description: A valid Polaris API key is required to establish a connection to the RTK corrections stream (polaris.pointonenav.com).
  docs: https://github.com/PointOneNav/polaris
  key_source: https://app.pointonenav.com
  type: apiKey
slug: pointonenav-authentication
source_filename: pointonenav-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: docs.pointonenav.com GraphQL API quickstart + github.com/PointOneNav/polaris\ndocs: https://docs.pointonenav.com/docs/graphql-api/quickstart\nsummary: >-\n  Point One services authenticate with an API key issued from the developer\n  portal at app.pointonenav.com. The same key model applies to the GraphQL API\n  and to the Polaris RTK Network Service.\nschemes:\n- api: Point One GraphQL API\n  type: apiKey\n  in: header\n  key_source: https://app.pointonenav.com\n  docs: https://docs.pointonenav.com/docs/graphql-api/quickstart\n  description: API-key authenticated GraphQL endpoint for workflow and data\n    management.\n- api: Polaris RTK Network Service\n  type: apiKey\n  key_source: https://app.pointonenav.com\n  docs: https://github.com/PointOneNav/polaris\n  description: A valid Polaris API key is required to establish a connection to the\n    RTK corrections stream (polaris.pointonenav.com).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pointonenav/refs/heads/main/authentication/pointonenav-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Positioning
- GNSS
- RTK
- Navigation
- Autonomous Vehicles
- Robotics
- Geolocation
- Sensor Fusion
---
