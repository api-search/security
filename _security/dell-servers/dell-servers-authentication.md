---
api_key_in:
- header
api_specs:
- filename: dell-servers-accounts-api-openapi.yml
  format: yaml
  label: Dell Servers Accounts API
  slug: dell-servers-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-accounts-api-openapi.yml
- filename: dell-servers-alerts-api-openapi.yml
  format: yaml
  label: Dell Servers Alerts API
  slug: dell-servers-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-alerts-api-openapi.yml
- filename: dell-servers-application-settings-api-openapi.yml
  format: yaml
  label: Dell Servers Application Settings API
  slug: dell-servers-application-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-application-settings-api-openapi.yml
- filename: dell-servers-chassis-api-openapi.yml
  format: yaml
  label: Dell Servers Chassis API
  slug: dell-servers-chassis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-chassis-api-openapi.yml
- filename: dell-servers-configuration-api-openapi.yml
  format: yaml
  label: Dell Servers Configuration API
  slug: dell-servers-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-configuration-api-openapi.yml
- filename: dell-servers-devices-api-openapi.yml
  format: yaml
  label: Dell Servers Devices API
  slug: dell-servers-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-devices-api-openapi.yml
- filename: dell-servers-discovery-api-openapi.yml
  format: yaml
  label: Dell Servers Discovery API
  slug: dell-servers-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-discovery-api-openapi.yml
- filename: dell-servers-event-service-api-openapi.yml
  format: yaml
  label: Dell Servers Event Service API
  slug: dell-servers-event-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-event-service-api-openapi.yml
- filename: dell-servers-firmware-api-openapi.yml
  format: yaml
  label: Dell Servers Firmware API
  slug: dell-servers-firmware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-firmware-api-openapi.yml
- filename: dell-servers-groups-api-openapi.yml
  format: yaml
  label: Dell Servers Groups API
  slug: dell-servers-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-groups-api-openapi.yml
- filename: dell-servers-jobs-api-openapi.yml
  format: yaml
  label: Dell Servers Jobs API
  slug: dell-servers-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-jobs-api-openapi.yml
- filename: dell-servers-managers-api-openapi.yml
  format: yaml
  label: Dell Servers Managers API
  slug: dell-servers-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-managers-api-openapi.yml
- filename: dell-servers-reports-api-openapi.yml
  format: yaml
  label: Dell Servers Reports API
  slug: dell-servers-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-reports-api-openapi.yml
- filename: dell-servers-service-root-api-openapi.yml
  format: yaml
  label: Dell Servers Service Root API
  slug: dell-servers-service-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-service-root-api-openapi.yml
- filename: dell-servers-sessions-api-openapi.yml
  format: yaml
  label: Dell Servers Sessions API
  slug: dell-servers-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-sessions-api-openapi.yml
- filename: dell-servers-systems-api-openapi.yml
  format: yaml
  label: Dell Servers Systems API
  slug: dell-servers-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-systems-api-openapi.yml
- filename: dell-servers-task-service-api-openapi.yml
  format: yaml
  label: Dell Servers Task Service API
  slug: dell-servers-task-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-task-service-api-openapi.yml
- filename: dell-servers-telemetry-service-api-openapi.yml
  format: yaml
  label: Dell Servers Telemetry Service API
  slug: dell-servers-telemetry-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-telemetry-service-api-openapi.yml
- filename: dell-servers-update-service-api-openapi.yml
  format: yaml
  label: Dell Servers Update Service API
  slug: dell-servers-update-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-update-service-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dell Servers Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dell Servers secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dell Servers
provider_slug: dell-servers
scheme_count: 2
schemes:
- description: HTTP Basic Authentication using iDRAC username and password credentials. All API requests require authentication except for the Redfish service root at /redfish/v1.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/dell-servers-idrac-redfish-openapi.yml
  type: http
- description: Session-based authentication using a token obtained from the Sessions resource POST operation. The token is passed in the X-Auth-Token header.
  in: header
  name: sessionAuth
  parameter: X-Auth-Token
  sources:
  - openapi/dell-servers-idrac-redfish-openapi.yml
  - openapi/dell-servers-openmanage-enterprise-openapi.yml
  type: apiKey
slug: dell-servers-authentication
source_filename: dell-servers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dell-servers-idrac-redfish-openapi.yml, openapi/dell-servers-openmanage-enterprise-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using iDRAC username and password credentials. All\n    API requests require authentication except for the Redfish service root at /redfish/v1.\n  sources:\n  - openapi/dell-servers-idrac-redfish-openapi.yml\n- name: sessionAuth\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: Session-based authentication using a token obtained from the Sessions resource\n    POST operation. The token is passed in the X-Auth-Token header.\n  sources:\n  - openapi/dell-servers-idrac-redfish-openapi.yml\n  - openapi/dell-servers-openmanage-enterprise-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/authentication/dell-servers-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Hardware
- Infrastructure
- Management
- Monitoring
- Servers
---
