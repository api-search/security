---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nist-cves-api-openapi.yml
  format: yaml
  label: National Institute of Standards and Technology (NIST) Cves API
  slug: nist-cves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nist/refs/heads/main/openapi/nist-cves-api-openapi.yml
- filename: nist-cve-history-api-openapi.yml
  format: yaml
  label: National Institute of Standards and Technology (NIST) CVE History API
  slug: nist-cve-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nist/refs/heads/main/openapi/nist-cve-history-api-openapi.yml
- filename: national-institute-of-standards-and-technology-cpe-api-openapi.yml
  format: yaml
  label: National Institute of Standards and Technology CPE API
  slug: national-institute-of-standards-and-technology-cpe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nist/refs/heads/main/openapi/national-institute-of-standards-and-technology-cpe-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
