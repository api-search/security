---
api_key_in: []
api_specs:
- filename: cisco-control-hub-adminauditevents-api-openapi.yml
  format: yaml
  label: Cisco Control Hub AdminAuditEvents API
  slug: cisco-control-hub-adminauditevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-adminauditevents-api-openapi.yml
- filename: cisco-control-hub-devices-api-openapi.yml
  format: yaml
  label: Cisco Control Hub Devices API
  slug: cisco-control-hub-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-devices-api-openapi.yml
- filename: cisco-control-hub-licenses-api-openapi.yml
  format: yaml
  label: Cisco Control Hub Licenses API
  slug: cisco-control-hub-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-licenses-api-openapi.yml
- filename: cisco-control-hub-locations-api-openapi.yml
  format: yaml
  label: Cisco Control Hub Locations API
  slug: cisco-control-hub-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-locations-api-openapi.yml
- filename: cisco-control-hub-organizations-api-openapi.yml
  format: yaml
  label: Cisco Control Hub Organizations API
  slug: cisco-control-hub-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-organizations-api-openapi.yml
- filename: cisco-control-hub-people-api-openapi.yml
  format: yaml
  label: Cisco Control Hub People API
  slug: cisco-control-hub-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-people-api-openapi.yml
- filename: cisco-control-hub-workspaces-api-openapi.yml
  format: yaml
  label: Cisco Control Hub Workspaces API
  slug: cisco-control-hub-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-workspaces-api-openapi.yml
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
