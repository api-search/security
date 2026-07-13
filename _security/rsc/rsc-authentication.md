---
api_key_in:
- header
api_specs:
- filename: rsc-chemspider-compounds-openapi.yml
  format: yaml
  label: ChemSpider Compounds API
  slug: chemspider-compounds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rsc/refs/heads/main/openapi/rsc-chemspider-compounds-openapi.yml
- filename: rsc-chemspider-compounds-openapi.yml
  format: yaml
  label: ChemSpider Tools API
  slug: chemspider-tools
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rsc/refs/heads/main/openapi/rsc-chemspider-compounds-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rsc Authentication
name_suffix: Authentication
oauth_flows: []
overview: RSC secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RSC
provider_slug: rsc
scheme_count: 1
schemes:
- description: API key obtained from the RSC Developer Portal at developer.rsc.org. Register and create an application to receive an API key.
  in: header
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/rsc-chemspider-compounds-openapi.yml
  type: apiKey
slug: rsc-authentication
source_filename: rsc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rsc-chemspider-compounds-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: API key obtained from the RSC Developer Portal at developer.rsc.org. Register\n    and create an application to receive an API key.\n  sources:\n  - openapi/rsc-chemspider-compounds-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rsc/refs/heads/main/authentication/rsc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Chemistry
- Cheminformatics
- Chemical Data
- Science
---
