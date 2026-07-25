---
api_key_in: []
api_specs:
- filename: paedae-applications-api-openapi.yml
  format: yaml
  label: Paedae Applications API
  slug: paedae-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-applications-api-openapi.yml
- filename: paedae-beacon-configurations-api-openapi.yml
  format: yaml
  label: Paedae Beacon Configurations API
  slug: paedae-beacon-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-beacon-configurations-api-openapi.yml
- filename: paedae-beacons-api-openapi.yml
  format: yaml
  label: Paedae Beacons API
  slug: paedae-beacons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-beacons-api-openapi.yml
- filename: paedae-communications-api-openapi.yml
  format: yaml
  label: Paedae Communications API
  slug: paedae-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-communications-api-openapi.yml
- filename: paedae-places-api-openapi.yml
  format: yaml
  label: Paedae Places API
  slug: paedae-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-places-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Paedae Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paedae declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Paedae
provider_slug: paedae
scheme_count: 2
schemes:
- applies_to: Manager REST API (applications, places, beacons, communications)
  description: 'Organization server API key issued in Gimbal Manager. Sent verbatim as `Authorization: Token token=<key>`.'
  format: Token token=my_organization_server_api_key
  header: Authorization
  id: OrganizationServerApiKey
  in: header
  type: apiKey
- applies_to: Select Proximity APIs
  authorization_url: https://manager.gimbal.com/oauth/authorize
  description: Some Proximity APIs require an OAuth 2.0 access token rather than the organization server API key. OAuth is also used by the Gimbal Manager portal login (manager.gimbal.com/auth/railsoauth).
  flow: authorizationCode
  id: ProximityOAuth2
  token_url: https://manager.gimbal.com/oauth/token
  type: oauth2
slug: paedae-authentication
source_filename: paedae-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.gimbal.com/rest.html\ntype: Authentication\nprovider: Paedae (Gimbal proximity platform)\nsummary: >-\n  The Gimbal REST API authenticates most requests with an organization server\n  API key passed in the Authorization header. Some Proximity APIs require an\n  OAuth 2.0 access token instead.\nschemes:\n  - id: OrganizationServerApiKey\n    type: apiKey\n    in: header\n    header: Authorization\n    format: 'Token token=my_organization_server_api_key'\n    description: >-\n      Organization server API key issued in Gimbal Manager. Sent verbatim as\n      `Authorization: Token token=<key>`.\n    applies_to: Manager REST API (applications, places, beacons, communications)\n  - id: ProximityOAuth2\n    type: oauth2\n    flow: authorizationCode\n    authorization_url: https://manager.gimbal.com/oauth/authorize\n    token_url: https://manager.gimbal.com/oauth/token\n    description: >-\n      Some Proximity APIs require\
  \ an OAuth 2.0 access token rather than the\n      organization server API key. OAuth is also used by the Gimbal Manager\n      portal login (manager.gimbal.com/auth/railsoauth).\n    applies_to: Select Proximity APIs\ncontent_type: application/json\ndocs: https://docs.gimbal.com/rest.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/authentication/paedae-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Proximity
- Location
- Beacons
- Geofencing
- Mobile SDK
- Advertising
- Marketing
---
