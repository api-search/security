---
api_key_in:
- header
api_specs:
- filename: nvd-cpe-api-openapi.yml
  format: yaml
  label: NVD CPE API
  slug: nvd-cpe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/openapi/nvd-cpe-api-openapi.yml
- filename: nvd-cpe-match-api-openapi.yml
  format: yaml
  label: NVD CPE Match API
  slug: nvd-cpe-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/openapi/nvd-cpe-match-api-openapi.yml
- filename: nvd-cve-api-openapi.yml
  format: yaml
  label: NVD CVE API
  slug: nvd-cve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/openapi/nvd-cve-api-openapi.yml
- filename: nvd-cve-change-history-api-openapi.yml
  format: yaml
  label: NVD CVE Change History API
  slug: nvd-cve-change-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/openapi/nvd-cve-change-history-api-openapi.yml
- filename: nvd-sources-api-openapi.yml
  format: yaml
  label: NVD Sources API
  slug: nvd-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/openapi/nvd-sources-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nvd Authentication
name_suffix: Authentication
oauth_flows: []
overview: NVD secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NVD
provider_slug: nvd
scheme_count: 1
schemes:
- description: 'NVD API key (optional but recommended). Without a key: 5 requests/30s. With a key: 50 requests/30s. Request at https://nvd.nist.gov/developers/request-an-api-key'
  in: header
  name: APIKey
  parameter: apiKey
  sources:
  - openapi/nvd-cve-openapi.yml
  type: apiKey
slug: nvd-authentication
source_filename: nvd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nvd-cve-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: 'NVD API key (optional but recommended). Without a key: 5 requests/30s. With\n    a key: 50 requests/30s. Request at https://nvd.nist.gov/developers/request-an-api-key'\n  sources:\n  - openapi/nvd-cve-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/authentication/nvd-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- CVE
- CPE
- Vulnerability
- CVSS
---
