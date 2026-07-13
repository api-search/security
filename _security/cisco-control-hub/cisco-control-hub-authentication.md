---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Webex Admin API
  slug: webex-admin-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Calling API
  slug: webex-calling-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Devices API
  slug: webex-devices-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Workspaces API
  slug: webex-workspaces-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex People API
  slug: webex-people-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Organizations API
  slug: webex-organizations-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Licenses API
  slug: webex-licenses-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Locations API
  slug: webex-locations-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Reports API
  slug: webex-reports-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Control Hub Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Control Hub secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cisco Control Hub
provider_slug: cisco-control-hub
scheme_count: 1
schemes:
- bearerFormat: OAuth2-Access-Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cisco-control-hub-openapi.yml
  type: http
slug: cisco-control-hub-authentication
source_filename: cisco-control-hub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-control-hub-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2-Access-Token\n  sources:\n  - openapi/cisco-control-hub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/authentication/cisco-control-hub-authentication.yml
summary_line: http · 1 scheme
tags:
- Administration
- Calling
- Collaboration
- Communications
- Device Management
- Identity Management
- Licenses
- Reporting
- Webex
---
