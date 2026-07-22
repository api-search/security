---
api_key_in:
- header
api_specs:
- filename: projectdiscovery-openapi-original.yml
  format: yaml
  label: ProjectDiscovery Cloud Platform (PDCP) API
  slug: projectdiscovery-cloud-platform-pdcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/projectdiscovery/refs/heads/main/openapi/projectdiscovery-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Projectdiscovery Authentication
name_suffix: Authentication
oauth_flows: []
overview: ProjectDiscovery secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ProjectDiscovery
provider_slug: projectdiscovery
scheme_count: 1
schemes:
- docs: https://cloud.projectdiscovery.io/settings/api-key
  in: header
  name: X-API-Key
  parameter: X-API-Key
  sources:
  - openapi/projectdiscovery-openapi-original.yml
  type: apiKey
slug: projectdiscovery-authentication
source_filename: projectdiscovery-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/projectdiscovery-openapi-original.yml\ndocs: https://docs.projectdiscovery.io/api-reference/introduction\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  The ProjectDiscovery Cloud Platform (PDCP) API authenticates every request\n  with an API key sent in the custom X-API-Key request header. Keys are created\n  and rotated from the cloud dashboard (Settings > API Key) or via the\n  /v1/user/apikey endpoints. All calls must be made over HTTPS. A small number\n  of leak-statistics endpoints (/v1/leaks/stats/domain, /v1/leaks/stats/email)\n  are public and require no authentication.\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  docs: https://cloud.projectdiscovery.io/settings/api-key\n  sources:\n  - openapi/projectdiscovery-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/projectdiscovery/refs/heads/main/authentication/projectdiscovery-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cybersecurity
- Security
- Vulnerability Scanning
- Attack Surface Management
- Vulnerability Management
- Asset Discovery
- DevSecOps
- Nuclei
- API
---
