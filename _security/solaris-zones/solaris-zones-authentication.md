---
api_key_in:
- cookie
api_specs:
- filename: solaris-zones-management-openapi.yml
  format: yaml
  label: Solaris Zones Management API
  slug: solaris-zones-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/openapi/solaris-zones-management-openapi.yml
- filename: solaris-zone-configuration-openapi.yml
  format: yaml
  label: Zone Configuration API
  slug: zone-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/openapi/solaris-zone-configuration-openapi.yml
- filename: solaris-zone-administration-openapi.yml
  format: yaml
  label: Zone Administration API
  slug: zone-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/openapi/solaris-zone-administration-openapi.yml
- filename: solaris-zone-monitoring-openapi.yml
  format: yaml
  label: Zone Monitoring API
  slug: zone-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/openapi/solaris-zone-monitoring-openapi.yml
- filename: solaris-rad-zonemgr-openapi.yml
  format: yaml
  label: RAD Zone Management REST API
  slug: rad-zone-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/openapi/solaris-rad-zonemgr-openapi.yml
- filename: solaris-zone-stats-openapi.yml
  format: yaml
  label: Zones Monitoring Statistics API (libzonestat)
  slug: zones-monitoring-statistics-api-libzonestat
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/openapi/solaris-zone-stats-openapi.yml
- filename: solaris-kernel-zones-openapi.yml
  format: yaml
  label: Oracle Solaris Kernel Zones API
  slug: oracle-solaris-kernel-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/openapi/solaris-kernel-zones-openapi.yml
- filename: solaris-statsstore-openapi.yml
  format: yaml
  label: Oracle Solaris StatsStore and Analytics API
  slug: oracle-solaris-statsstore-and-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/openapi/solaris-statsstore-openapi.yml
- filename: solaris-unified-archives-openapi.yml
  format: yaml
  label: Oracle Solaris Unified Archives Zones API
  slug: oracle-solaris-unified-archives-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/openapi/solaris-unified-archives-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Solaris Zones Authentication
name_suffix: Authentication
oauth_flows: []
overview: Solaris Zones secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Solaris Zones
provider_slug: solaris-zones
scheme_count: 2
schemes:
- description: RAD session cookie obtained via authentication
  in: cookie
  name: cookieAuth
  parameter: _rad_session
  sources:
  - openapi/solaris-kernel-zones-openapi.yml
  - openapi/solaris-statsstore-openapi.yml
  - openapi/solaris-unified-archives-openapi.yml
  - openapi/solaris-zone-administration-openapi.yml
  - openapi/solaris-zone-configuration-openapi.yml
  - openapi/solaris-zone-monitoring-openapi.yml
  - openapi/solaris-zone-stats-openapi.yml
  - openapi/solaris-zones-management-openapi.yml
  type: apiKey
- description: RAD session cookie obtained through authentication. Use the RAD authentication endpoint to establish a session and obtain the cookie.
  in: cookie
  name: cookieAuth
  parameter: _rad_cookie
  sources:
  - openapi/solaris-rad-zonemgr-openapi.yml
  type: apiKey
slug: solaris-zones-authentication
source_filename: solaris-zones-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/solaris-kernel-zones-openapi.yml, openapi/solaris-rad-zonemgr-openapi.yml, openapi/solaris-statsstore-openapi.yml,\n  openapi/solaris-unified-archives-openapi.yml, openapi/solaris-zone-administration-openapi.yml,\n  openapi/solaris-zone-configuration-openapi.yml, openapi/solaris-zone-monitoring-openapi.yml,\n  openapi/solaris-zone-stats-openapi.yml, openapi/solaris-zones-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: _rad_session\n  description: RAD session cookie obtained via authentication\n  sources:\n  - openapi/solaris-kernel-zones-openapi.yml\n  - openapi/solaris-statsstore-openapi.yml\n  - openapi/solaris-unified-archives-openapi.yml\n  - openapi/solaris-zone-administration-openapi.yml\n  - openapi/solaris-zone-configuration-openapi.yml\n  - openapi/solaris-zone-monitoring-openapi.yml\n  - openapi/solaris-zone-stats-openapi.yml\n\
  \  - openapi/solaris-zones-management-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: _rad_cookie\n  description: RAD session cookie obtained through authentication. Use the RAD authentication\n    endpoint to establish a session and obtain the cookie.\n  sources:\n  - openapi/solaris-rad-zonemgr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/authentication/solaris-zones-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Containers
- Kernel Zones
- Operating Systems
- Oracle
- RAD
- Resource Management
- Solaris
- StatsStore
- Virtualization
- Zones
---
