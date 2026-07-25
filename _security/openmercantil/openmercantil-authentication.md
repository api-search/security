---
api_key_in:
- cookie
api_specs:
- filename: openmercantil-billing-api-openapi.yml
  format: yaml
  label: OpenMercantil Billing API
  slug: openmercantil-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-billing-api-openapi.yml
- filename: openmercantil-companies-api-openapi.yml
  format: yaml
  label: OpenMercantil Companies API
  slug: openmercantil-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-companies-api-openapi.yml
- filename: openmercantil-contracts-api-openapi.yml
  format: yaml
  label: OpenMercantil Contracts API
  slug: openmercantil-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-contracts-api-openapi.yml
- filename: openmercantil-daily-api-openapi.yml
  format: yaml
  label: OpenMercantil Daily API
  slug: openmercantil-daily-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-daily-api-openapi.yml
- filename: openmercantil-export-api-openapi.yml
  format: yaml
  label: OpenMercantil Export API
  slug: openmercantil-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-export-api-openapi.yml
- filename: openmercantil-geocode-api-openapi.yml
  format: yaml
  label: OpenMercantil Geocode API
  slug: openmercantil-geocode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-geocode-api-openapi.yml
- filename: openmercantil-network-api-openapi.yml
  format: yaml
  label: OpenMercantil Network API
  slug: openmercantil-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-network-api-openapi.yml
- filename: openmercantil-persons-api-openapi.yml
  format: yaml
  label: OpenMercantil Persons API
  slug: openmercantil-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-persons-api-openapi.yml
- filename: openmercantil-score-api-openapi.yml
  format: yaml
  label: OpenMercantil Score API
  slug: openmercantil-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-score-api-openapi.yml
- filename: openmercantil-search-api-openapi.yml
  format: yaml
  label: OpenMercantil Search API
  slug: openmercantil-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-search-api-openapi.yml
- filename: openmercantil-sectors-api-openapi.yml
  format: yaml
  label: OpenMercantil Sectors API
  slug: openmercantil-sectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-sectors-api-openapi.yml
- filename: openmercantil-sources-api-openapi.yml
  format: yaml
  label: OpenMercantil Sources API
  slug: openmercantil-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-sources-api-openapi.yml
- filename: openmercantil-stats-api-openapi.yml
  format: yaml
  label: OpenMercantil Stats API
  slug: openmercantil-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-stats-api-openapi.yml
- filename: openmercantil-system-api-openapi.yml
  format: yaml
  label: OpenMercantil System API
  slug: openmercantil-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-system-api-openapi.yml
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
