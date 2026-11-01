---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flashodds-live-api-openapi.json
  format: json
  label: Sorqen API API
  slug: sorqen-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashodds-live/openapi/_original/flashodds-live-api-openapi.json
auth_types: []
description: Client authenticates by providing a bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Flashodds Live Authentication
name_suffix: Authentication
oauth_flows: []
overview: flashodds-live declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: flashodds-live
provider_slug: flashodds-live
scheme_count: 1
schemes:
- evidence: 'Copy claude mcp add --transport http flash-props https://api.flashodds.live/mcp --header "Authorization: Bearer YOUR_KEY"'
  header: Authorization
  how_to_obtain: Obtain a free or paid API key from the Flash Props page and use it as the bearer token.
  location: header
  name: Bearer token
  type: http-bearer
slug: flashodds-live-authentication
source_filename: flashodds-live-authentication.yml
source_heading: Authentication Profile
source_url: https://api.flashodds.live/connect
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.flashodds.live/connect\nsources:\n- https://api.flashodds.live/connect\ndescription: Client authenticates by providing a bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Copy claude mcp add --transport http flash-props https://api.flashodds.live/mcp --header \"Authorization: Bearer YOUR_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a free or paid API key from the Flash Props page and use it as the bearer token.\ndocs: https://api.flashodds.live/connect\n"
source_yaml_url: https://artifacts.apis.io/flashodds-live/authentication/flashodds-live-authentication.yml
summary_line: 1 scheme
tags:
- Sports
- Betting
- Odds
- Real-time
- Analytics
- API
---
