---
anonymous_access: false
api_key_in: []
api_specs:
- filename: engrate-audit-logs-api-openapi.yml
  format: yaml
  label: Engrate Audit Logs API
  slug: engrate-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-audit-logs-api-openapi.yml
- filename: engrate-benachrichtigung-api-openapi.yml
  format: yaml
  label: Engrate Benachrichtigung API
  slug: engrate-benachrichtigung-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-benachrichtigung-api-openapi.yml
- filename: engrate-betrieb-api-openapi.yml
  format: yaml
  label: Engrate Betrieb API
  slug: engrate-betrieb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-betrieb-api-openapi.yml
- filename: engrate-clearing-api-openapi.yml
  format: yaml
  label: Engrate Clearing API
  slug: engrate-clearing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-clearing-api-openapi.yml
- filename: engrate-core-api-openapi.yml
  format: yaml
  label: Engrate Core API
  slug: engrate-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-core-api-openapi.yml
- filename: engrate-cost-of-energy-api-openapi.yml
  format: yaml
  label: Engrate Cost Of Energy API
  slug: engrate-cost-of-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-cost-of-energy-api-openapi.yml
- filename: engrate-geo-api-openapi.yml
  format: yaml
  label: Engrate Geo API
  slug: engrate-geo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-geo-api-openapi.yml
- filename: engrate-holidays-api-openapi.yml
  format: yaml
  label: Engrate Holidays API
  slug: engrate-holidays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-holidays-api-openapi.yml
- filename: engrate-lokationen-api-openapi.yml
  format: yaml
  label: Engrate Lokationen API
  slug: engrate-lokationen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-lokationen-api-openapi.yml
- filename: engrate-lokationsb-ndel-api-openapi.yml
  format: yaml
  label: Engrate Lokationsbündel API
  slug: engrate-lokationsb-ndel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-lokationsb-ndel-api-openapi.yml
- filename: engrate-mabis-api-openapi.yml
  format: yaml
  label: Engrate Mabis API
  slug: engrate-mabis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-mabis-api-openapi.yml
- filename: engrate-netzbetreiberwechsel-api-openapi.yml
  format: yaml
  label: Engrate Netzbetreiberwechsel API
  slug: engrate-netzbetreiberwechsel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-netzbetreiberwechsel-api-openapi.yml
- filename: engrate-nl-settlement-api-openapi.yml
  format: yaml
  label: Engrate Nl Settlement API
  slug: engrate-nl-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-nl-settlement-api-openapi.yml
- filename: engrate-profiles-api-openapi.yml
  format: yaml
  label: Engrate Profiles API
  slug: engrate-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-profiles-api-openapi.yml
- filename: engrate-reference-api-openapi.yml
  format: yaml
  label: Engrate Reference API
  slug: engrate-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-reference-api-openapi.yml
- filename: engrate-schedules-api-openapi.yml
  format: yaml
  label: Engrate Schedules API
  slug: engrate-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-schedules-api-openapi.yml
- filename: engrate-status-request-api-openapi.yml
  format: yaml
  label: Engrate Status Request API
  slug: engrate-status-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-status-request-api-openapi.yml
- filename: engrate-time-series-api-openapi.yml
  format: yaml
  label: Engrate Time Series API
  slug: engrate-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-time-series-api-openapi.yml
auth_types: []
description: Authentication using API keys
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Engrate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Engrate declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Engrate
provider_slug: engrate
scheme_count: 1
schemes:
- evidence: This guide explains how to authenticate with our API using API keys.
  header: authorization
  how_to_obtain: Create an API key at https://console.engrate.io
  location: header
  name: API Key
  type: apiKey
slug: engrate-authentication
source_filename: engrate-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.engrate.io/guides/authentication.md
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.engrate.io/guides/authentication.md\nsources:\n- https://docs.engrate.io/guides/authentication.md\n- https://docs.engrate.io/guides/cost-of-energy-quickstart.md\ndescription: Authentication using API keys\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: This guide explains how to authenticate with our API using API keys.\n  location: header\n  header: authorization\n  how_to_obtain: Create an API key at https://console.engrate.io\ndocs: https://docs.engrate.io/guides/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/authentication/engrate-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Energy
- Platform
- Integration
- Market
---
