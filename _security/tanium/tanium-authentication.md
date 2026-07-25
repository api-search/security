---
api_key_in:
- header
api_specs:
- filename: tanium-actions-api-openapi.yml
  format: yaml
  label: Tanium Actions API
  slug: tanium-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-actions-api-openapi.yml
- filename: tanium-alerts-api-openapi.yml
  format: yaml
  label: Tanium Alerts API
  slug: tanium-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-alerts-api-openapi.yml
- filename: tanium-authentication-api-openapi.yml
  format: yaml
  label: Tanium Authentication API
  slug: tanium-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-authentication-api-openapi.yml
- filename: tanium-connections-api-openapi.yml
  format: yaml
  label: Tanium Connections API
  slug: tanium-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-connections-api-openapi.yml
- filename: tanium-destinations-api-openapi.yml
  format: yaml
  label: Tanium Destinations API
  slug: tanium-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-destinations-api-openapi.yml
- filename: tanium-events-api-openapi.yml
  format: yaml
  label: Tanium Events API
  slug: tanium-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-events-api-openapi.yml
- filename: tanium-evidence-api-openapi.yml
  format: yaml
  label: Tanium Evidence API
  slug: tanium-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-evidence-api-openapi.yml
- filename: tanium-file-downloads-api-openapi.yml
  format: yaml
  label: Tanium File Downloads API
  slug: tanium-file-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-file-downloads-api-openapi.yml
- filename: tanium-file-operations-api-openapi.yml
  format: yaml
  label: Tanium File Operations API
  slug: tanium-file-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-file-operations-api-openapi.yml
- filename: tanium-groups-api-openapi.yml
  format: yaml
  label: Tanium Groups API
  slug: tanium-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-groups-api-openapi.yml
- filename: tanium-intel-documents-api-openapi.yml
  format: yaml
  label: Tanium Intel Documents API
  slug: tanium-intel-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-intel-documents-api-openapi.yml
- filename: tanium-labels-api-openapi.yml
  format: yaml
  label: Tanium Labels API
  slug: tanium-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-labels-api-openapi.yml
- filename: tanium-packages-api-openapi.yml
  format: yaml
  label: Tanium Packages API
  slug: tanium-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-packages-api-openapi.yml
- filename: tanium-processes-api-openapi.yml
  format: yaml
  label: Tanium Processes API
  slug: tanium-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-processes-api-openapi.yml
- filename: tanium-questions-api-openapi.yml
  format: yaml
  label: Tanium Questions API
  slug: tanium-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-questions-api-openapi.yml
- filename: tanium-saved-questions-api-openapi.yml
  format: yaml
  label: Tanium Saved Questions API
  slug: tanium-saved-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-saved-questions-api-openapi.yml
- filename: tanium-schedules-api-openapi.yml
  format: yaml
  label: Tanium Schedules API
  slug: tanium-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-schedules-api-openapi.yml
- filename: tanium-sensors-api-openapi.yml
  format: yaml
  label: Tanium Sensors API
  slug: tanium-sensors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-sensors-api-openapi.yml
- filename: tanium-snapshots-api-openapi.yml
  format: yaml
  label: Tanium Snapshots API
  slug: tanium-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-snapshots-api-openapi.yml
- filename: tanium-sources-api-openapi.yml
  format: yaml
  label: Tanium Sources API
  slug: tanium-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-sources-api-openapi.yml
- filename: tanium-status-api-openapi.yml
  format: yaml
  label: Tanium Status API
  slug: tanium-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/openapi/tanium-status-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tanium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tanium secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tanium
provider_slug: tanium
scheme_count: 1
schemes:
- description: API token passed in the session header for authenticating with the Tanium Connect API.
  in: header
  name: apiToken
  parameter: session
  sources:
  - openapi/tanium-connect-api-openapi.yml
  - openapi/tanium-platform-rest-api-openapi.yml
  - openapi/tanium-threat-response-api-openapi.yml
  type: apiKey
slug: tanium-authentication
source_filename: tanium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tanium-connect-api-openapi.yml, openapi/tanium-platform-rest-api-openapi.yml,\n  openapi/tanium-threat-response-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: session\n  description: API token passed in the session header for authenticating with the Tanium Connect\n    API.\n  sources:\n  - openapi/tanium-connect-api-openapi.yml\n  - openapi/tanium-platform-rest-api-openapi.yml\n  - openapi/tanium-threat-response-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/authentication/tanium-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Compliance
- Endpoint Management
- Patch Management
- Security
- Threat Detection
- Unified Endpoint Management
---
