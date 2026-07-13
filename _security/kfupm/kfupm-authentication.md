---
api_key_in:
- header
api_specs:
- filename: oai2
  format: yaml
  label: KFUPM ePrints OAI-PMH
  slug: eprints-oai
  spec_type: OpenAPI
  url: https://eprints.kfupm.edu.sa/cgi/oai2?verb=Identify
- filename: kfupm-pure-ws.yaml
  format: yaml
  label: KFUPM Pure Web Services API
  slug: pure-ws
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/openapi/kfupm-pure-ws.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kfupm Authentication
name_suffix: Authentication
oauth_flows: []
overview: King Fahd University of Petroleum & Minerals secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: King Fahd University of Petroleum & Minerals
provider_slug: kfupm
scheme_count: 1
schemes:
- description: Security mechanism for the API
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/kfupm-pure-ws.yaml
  type: apiKey
slug: kfupm-authentication
source_filename: kfupm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kfupm-pure-ws.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Security mechanism for the API\n  sources:\n  - openapi/kfupm-pure-ws.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/authentication/kfupm-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Repository
- Saudi Arabia
- Middle East
---
