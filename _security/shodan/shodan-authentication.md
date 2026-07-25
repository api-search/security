---
api_key_in:
- query
api_specs:
- filename: shodan-account-api-openapi.yml
  format: yaml
  label: Shodan Account API
  slug: shodan-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-account-api-openapi.yml
- filename: shodan-bulk-data-api-openapi.yml
  format: yaml
  label: Shodan Bulk Data API
  slug: shodan-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-bulk-data-api-openapi.yml
- filename: shodan-cpe-api-openapi.yml
  format: yaml
  label: Shodan CPE API
  slug: shodan-cpe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-cpe-api-openapi.yml
- filename: shodan-cve-api-openapi.yml
  format: yaml
  label: Shodan CVE API
  slug: shodan-cve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-cve-api-openapi.yml
- filename: shodan-directory-api-openapi.yml
  format: yaml
  label: Shodan Directory API
  slug: shodan-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-directory-api-openapi.yml
- filename: shodan-dns-api-openapi.yml
  format: yaml
  label: Shodan DNS API
  slug: shodan-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-dns-api-openapi.yml
- filename: shodan-internetdb-api-openapi.yml
  format: yaml
  label: Shodan InternetDB API
  slug: shodan-internetdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-internetdb-api-openapi.yml
- filename: shodan-network-alerts-api-openapi.yml
  format: yaml
  label: Shodan Network Alerts API
  slug: shodan-network-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-network-alerts-api-openapi.yml
- filename: shodan-notifiers-api-openapi.yml
  format: yaml
  label: Shodan Notifiers API
  slug: shodan-notifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-notifiers-api-openapi.yml
- filename: shodan-on-demand-scanning-api-openapi.yml
  format: yaml
  label: Shodan On-Demand Scanning API
  slug: shodan-on-demand-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-on-demand-scanning-api-openapi.yml
- filename: shodan-organization-api-openapi.yml
  format: yaml
  label: Shodan Organization API
  slug: shodan-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-organization-api-openapi.yml
- filename: shodan-search-methods-api-openapi.yml
  format: yaml
  label: Shodan Search Methods API
  slug: shodan-search-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-search-methods-api-openapi.yml
- filename: shodan-streaming-api-openapi.yml
  format: yaml
  label: Shodan Streaming API
  slug: shodan-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-streaming-api-openapi.yml
- filename: shodan-trends-api-openapi.yml
  format: yaml
  label: Shodan Trends API
  slug: shodan-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-trends-api-openapi.yml
- filename: shodan-utility-api-openapi.yml
  format: yaml
  label: Shodan Utility API
  slug: shodan-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-utility-api-openapi.yml
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
