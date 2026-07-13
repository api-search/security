---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: TimezoneDB API
  slug: timezonedb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timezonedb/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Timezonedb Authentication
name_suffix: Authentication
oauth_flows: []
overview: TimezoneDB secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TimezoneDB
provider_slug: timezonedb
scheme_count: 1
schemes:
- description: API key obtained from https://timezonedb.com/register
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: timezonedb-authentication
source_filename: timezonedb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key obtained from https://timezonedb.com/register\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timezonedb/refs/heads/main/authentication/timezonedb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Timezone
- Time
- Geographic Coordinates
- DST
- UTC Offset
- Time Conversion
- Location
---
