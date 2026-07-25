---
api_key_in:
- query
api_specs:
- filename: datalastic-historical-api-openapi.yml
  format: yaml
  label: Datalastic Historical API
  slug: datalastic-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-historical-api-openapi.yml
- filename: datalastic-live-tracking-api-openapi.yml
  format: yaml
  label: Datalastic Live Tracking API
  slug: datalastic-live-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-live-tracking-api-openapi.yml
- filename: datalastic-ports-api-openapi.yml
  format: yaml
  label: Datalastic Ports API
  slug: datalastic-ports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-ports-api-openapi.yml
- filename: datalastic-reports-and-usage-api-openapi.yml
  format: yaml
  label: Datalastic Reports and Usage API
  slug: datalastic-reports-and-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-reports-and-usage-api-openapi.yml
- filename: datalastic-vessel-data-api-openapi.yml
  format: yaml
  label: Datalastic Vessel Data API
  slug: datalastic-vessel-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-vessel-data-api-openapi.yml
- filename: datalastic-zone-traffic-api-openapi.yml
  format: yaml
  label: Datalastic Zone Traffic API
  slug: datalastic-zone-traffic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-zone-traffic-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Datalastic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datalastic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Datalastic
provider_slug: datalastic
scheme_count: 1
schemes:
- description: Personal API key issued with a Datalastic subscription. Passed as the api-key query parameter on every request.
  in: query
  name: apiKey
  parameter: api-key
  sources:
  - openapi/datalastic-openapi.yml
  type: apiKey
slug: datalastic-authentication
source_filename: datalastic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datalastic-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api-key\n  description: Personal API key issued with a Datalastic subscription. Passed as the api-key\n    query parameter on every request.\n  sources:\n  - openapi/datalastic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/authentication/datalastic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Vessel Tracking
- Maritime
- AIS
- Ships
- Ports
- Shipping
---
