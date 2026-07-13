---
api_key_in:
- header
api_specs:
- filename: nist-nvd-cve-openapi.yml
  format: yaml
  label: NIST National Vulnerability Database (NVD) API
  slug: nist-nvd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nist/refs/heads/main/openapi/nist-nvd-cve-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nist Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Institute of Standards and Technology (NIST) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: National Institute of Standards and Technology (NIST)
provider_slug: nist
scheme_count: 1
schemes:
- description: Optional API key obtained from https://nvd.nist.gov/developers/request-an-api-key. Increases rate limits.
  in: header
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/nist-nvd-cve-openapi.yml
  type: apiKey
slug: nist-authentication
source_filename: nist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nist-nvd-cve-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: Optional API key obtained from https://nvd.nist.gov/developers/request-an-api-key.\n    Increases rate limits.\n  sources:\n  - openapi/nist-nvd-cve-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nist/refs/heads/main/authentication/nist-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cybersecurity
- Government
- Measurements
- Research
- Scientific Data
- Standards
---
