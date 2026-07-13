---
api_key_in:
- query
api_specs:
- filename: shodan-rest-openapi.yml
  format: yaml
  label: Shodan REST API
  slug: shodan-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-rest-openapi.yml
- filename: shodan-stream-openapi.yml
  format: yaml
  label: Shodan Streaming API
  slug: shodan-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-stream-openapi.yml
- filename: shodan-trends-openapi.yml
  format: yaml
  label: Shodan Trends API
  slug: shodan-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-trends-openapi.yml
- filename: shodan-internetdb-openapi.yml
  format: yaml
  label: InternetDB API
  slug: internetdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-internetdb-openapi.yml
- filename: shodan-cvedb-openapi.yml
  format: yaml
  label: CVEDB API
  slug: cvedb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-cvedb-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shodan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shodan secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shodan
provider_slug: shodan
scheme_count: 1
schemes:
- description: Shodan API key.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/shodan-rest-openapi.yml
  - openapi/shodan-stream-openapi.yml
  - openapi/shodan-trends-openapi.yml
  type: apiKey
slug: shodan-authentication
source_filename: shodan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shodan-rest-openapi.yml, openapi/shodan-stream-openapi.yml, openapi/shodan-trends-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Shodan API key.\n  sources:\n  - openapi/shodan-rest-openapi.yml\n  - openapi/shodan-stream-openapi.yml\n  - openapi/shodan-trends-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/authentication/shodan-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Search
- Internet
- Devices
- IoT
- Vulnerabilities
- CVE
- Attack Surface
- Threat Intelligence
- Reconnaissance
- Network
- DNS
- Scanning
- Public APIs
---
