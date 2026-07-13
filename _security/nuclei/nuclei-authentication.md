---
api_key_in:
- header
api_specs:
- filename: nuclei-openapi.yml
  format: yaml
  label: Nuclei
  slug: nuclei
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclei/refs/heads/main/openapi/nuclei-openapi.yml
- filename: nuclei-openapi.yml
  format: yaml
  label: ProjectDiscovery Cloud Platform API
  slug: projectdiscovery-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclei/refs/heads/main/openapi/nuclei-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nuclei Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuclei secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nuclei
provider_slug: nuclei
scheme_count: 1
schemes:
- in: header
  name: X-API-Key
  parameter: X-API-Key
  sources:
  - openapi/nuclei-openapi.yml
  type: apiKey
slug: nuclei-authentication
source_filename: nuclei-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nuclei-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/nuclei-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuclei/refs/heads/main/authentication/nuclei-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security Testing
- Testing
- Vulnerability Scanner
- DAST
- Open Source
---
