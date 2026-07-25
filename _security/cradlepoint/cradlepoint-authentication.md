---
api_key_in:
- header
api_specs:
- filename: cradlepoint-accounts-api-openapi.yml
  format: yaml
  label: Cradlepoint Accounts API
  slug: cradlepoint-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cradlepoint/refs/heads/main/openapi/cradlepoint-accounts-api-openapi.yml
- filename: cradlepoint-activitylogs-api-openapi.yml
  format: yaml
  label: Cradlepoint ActivityLogs API
  slug: cradlepoint-activitylogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cradlepoint/refs/heads/main/openapi/cradlepoint-activitylogs-api-openapi.yml
- filename: cradlepoint-alertpushdestinations-api-openapi.yml
  format: yaml
  label: Cradlepoint AlertPushDestinations API
  slug: cradlepoint-alertpushdestinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cradlepoint/refs/heads/main/openapi/cradlepoint-alertpushdestinations-api-openapi.yml
- filename: cradlepoint-alertrules-api-openapi.yml
  format: yaml
  label: Cradlepoint AlertRules API
  slug: cradlepoint-alertrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cradlepoint/refs/heads/main/openapi/cradlepoint-alertrules-api-openapi.yml
- filename: cradlepoint-alerts-api-openapi.yml
  format: yaml
  label: Cradlepoint Alerts API
  slug: cradlepoint-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cradlepoint/refs/heads/main/openapi/cradlepoint-alerts-api-openapi.yml
- filename: cradlepoint-groups-api-openapi.yml
  format: yaml
  label: Cradlepoint Groups API
  slug: cradlepoint-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cradlepoint/refs/heads/main/openapi/cradlepoint-groups-api-openapi.yml
- filename: cradlepoint-locations-api-openapi.yml
  format: yaml
  label: Cradlepoint Locations API
  slug: cradlepoint-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cradlepoint/refs/heads/main/openapi/cradlepoint-locations-api-openapi.yml
- filename: cradlepoint-netdevices-api-openapi.yml
  format: yaml
  label: Cradlepoint NetDevices API
  slug: cradlepoint-netdevices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cradlepoint/refs/heads/main/openapi/cradlepoint-netdevices-api-openapi.yml
- filename: cradlepoint-routers-api-openapi.yml
  format: yaml
  label: Cradlepoint Routers API
  slug: cradlepoint-routers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cradlepoint/refs/heads/main/openapi/cradlepoint-routers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cradlepoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cradlepoint secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cradlepoint
provider_slug: cradlepoint
scheme_count: 2
schemes:
- description: Cradlepoint account API ID (paired with X-CP-API-KEY).
  in: header
  name: CradlepointApiKey
  parameter: X-CP-API-ID
  sources:
  - openapi/cradlepoint-netcloud-manager-api-v2-openapi.yml
  type: apiKey
- description: NCM tenant API ID (paired with X-ECM-API-KEY), carries the NCM role.
  in: header
  name: NetCloudApiKey
  parameter: X-ECM-API-ID
  sources:
  - openapi/cradlepoint-netcloud-manager-api-v2-openapi.yml
  type: apiKey
slug: cradlepoint-authentication
source_filename: cradlepoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cradlepoint-netcloud-manager-api-v2-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: CradlepointApiKey\n  type: apiKey\n  in: header\n  parameter: X-CP-API-ID\n  description: Cradlepoint account API ID (paired with X-CP-API-KEY).\n  sources:\n  - openapi/cradlepoint-netcloud-manager-api-v2-openapi.yml\n- name: NetCloudApiKey\n  type: apiKey\n  in: header\n  parameter: X-ECM-API-ID\n  description: NCM tenant API ID (paired with X-ECM-API-KEY), carries the NCM role.\n  sources:\n  - openapi/cradlepoint-netcloud-manager-api-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cradlepoint/refs/heads/main/authentication/cradlepoint-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Wireless WAN
- 5G
- LTE
- Edge
- Branch Networking
- SD-WAN
- SASE
- Routers
- In-Vehicle
- IoT
- Cellular
- Private 5G
- NetCloud
- Ericsson
---
