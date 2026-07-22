---
api_key_in:
- query
api_specs:
- filename: solaredge-monitoring-openapi.yml
  format: yaml
  label: SolarEdge Monitoring API
  slug: solaredge-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solaredge/refs/heads/main/openapi/solaredge-monitoring-openapi.yml
auth_types:
- apiKey
description: The SolarEdge Monitoring API authenticates every request with a single API key passed as the api_key query parameter. Keys are generated inside the SolarEdge monitoring platform under Admin > Site Access > API Access and are scoped to the account (and the sites it can access). There is no OAuth2/OIDC surface. Verified live against https://monitoringapi.solaredge.com/version/current and /sites/list?api_key=INVALID, both of which return an RFC 9457 problem+json body with title "Unauthorized - Authentication Failed" / detail "Invalid API key" (HTTP 401) when the key is missing or wrong.
kind: authentication
layout: security
method: searched
name: Solaredge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Solaredge secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Solaredge
provider_slug: solaredge
scheme_count: 1
schemes:
- description: Account API key generated in the SolarEdge monitoring platform (Admin > Site Access > API Access). Required on every endpoint.
  evidence:
  - status: 401
    url: https://monitoringapi.solaredge.com/version/current
  - body: RFC 9457 problem+json, detail "Invalid API key"
    status: 401
    url: https://monitoringapi.solaredge.com/sites/list?api_key=INVALID
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/solaredge-monitoring-openapi.yml
  type: apiKey
slug: solaredge-authentication
source_filename: solaredge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api-docs.solaredge.com/\ndocs: https://api-docs.solaredge.com/\ndescription: >-\n  The SolarEdge Monitoring API authenticates every request with a single API key\n  passed as the api_key query parameter. Keys are generated inside the SolarEdge\n  monitoring platform under Admin > Site Access > API Access and are scoped to the\n  account (and the sites it can access). There is no OAuth2/OIDC surface. Verified\n  live against https://monitoringapi.solaredge.com/version/current and\n  /sites/list?api_key=INVALID, both of which return an RFC 9457 problem+json body\n  with title \"Unauthorized - Authentication Failed\" / detail \"Invalid API key\"\n  (HTTP 401) when the key is missing or wrong.\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\nschemes:\n  - name: api_key\n    type: apiKey\n    in: query\n    parameter: api_key\n    description: >-\n      Account API key generated in the SolarEdge monitoring\
  \ platform\n      (Admin > Site Access > API Access). Required on every endpoint.\n    sources:\n      - openapi/solaredge-monitoring-openapi.yml\n    evidence:\n      - {url: 'https://monitoringapi.solaredge.com/version/current', status: 401}\n      - {url: 'https://monitoringapi.solaredge.com/sites/list?api_key=INVALID', status: 401, body: 'RFC 9457 problem+json, detail \"Invalid API key\"'}\nnotes: >-\n  The api_key travels in the URL query string, so it is exposed in server logs and\n  browser history; SolarEdge documents rotating/regenerating the key from the\n  monitoring platform. No refresh-token or scope model exists.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solaredge/refs/heads/main/authentication/solaredge-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Solar Energy
- Photovoltaic
- Energy Monitoring
- IoT
- Renewable Energy
- Inverters
- Energy Storage
---
