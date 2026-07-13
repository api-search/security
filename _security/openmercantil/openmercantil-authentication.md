---
api_key_in:
- cookie
api_specs:
- filename: openmercantil-openapi.yml
  format: yaml
  label: OpenMercantil Public API
  slug: openmercantil-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openmercantil Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenMercantil secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenMercantil
provider_slug: openmercantil
scheme_count: 1
schemes:
- description: Session cookie issued after web sign-in, required only for billing endpoints.
  in: cookie
  name: sessionCookie
  parameter: session
  sources:
  - openapi/openmercantil-openapi.yml
  type: apiKey
slug: openmercantil-authentication
source_filename: openmercantil-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openmercantil-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: session\n  description: Session cookie issued after web sign-in, required only for billing endpoints.\n  sources:\n  - openapi/openmercantil-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/authentication/openmercantil-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Open Data
- Spain
- Company Data
- Business Registry
- BORME
- Public Records
- Spanish Companies
- CIF
- CNAE
- Public Procurement
- PLACSP
- CNMV
- OEPM
- BDNS
- OpenSanctions
- Public-Interest Data
- Spanish Open Data
- REST API
- JSON
- CSV
- Geocoding
- Trust Score
- Registry Timeline
- Daily Summary
---
