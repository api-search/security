---
api_key_in: []
api_specs:
- filename: mark43-associated-records-api-openapi.yml
  format: yaml
  label: Mark43 Associated Records API
  slug: mark43-associated-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-associated-records-api-openapi.yml
- filename: mark43-attachments-api-openapi.yml
  format: yaml
  label: Mark43 Attachments API
  slug: mark43-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-attachments-api-openapi.yml
- filename: mark43-cad-configuration-api-openapi.yml
  format: yaml
  label: Mark43 CAD Configuration API
  slug: mark43-cad-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-cad-configuration-api-openapi.yml
- filename: mark43-cad-events-api-openapi.yml
  format: yaml
  label: Mark43 CAD Events API
  slug: mark43-cad-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-cad-events-api-openapi.yml
- filename: mark43-cad-tickets-api-openapi.yml
  format: yaml
  label: Mark43 CAD Tickets API
  slug: mark43-cad-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-cad-tickets-api-openapi.yml
- filename: mark43-cases-api-openapi.yml
  format: yaml
  label: Mark43 Cases API
  slug: mark43-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-cases-api-openapi.yml
- filename: mark43-e911-api-openapi.yml
  format: yaml
  label: Mark43 E911 API
  slug: mark43-e911-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-e911-api-openapi.yml
- filename: mark43-evidence-api-openapi.yml
  format: yaml
  label: Mark43 Evidence API
  slug: mark43-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-evidence-api-openapi.yml
- filename: mark43-gps-api-openapi.yml
  format: yaml
  label: Mark43 GPS API
  slug: mark43-gps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-gps-api-openapi.yml
- filename: mark43-persons-api-openapi.yml
  format: yaml
  label: Mark43 Persons API
  slug: mark43-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-persons-api-openapi.yml
- filename: mark43-reports-api-openapi.yml
  format: yaml
  label: Mark43 Reports API
  slug: mark43-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-reports-api-openapi.yml
- filename: mark43-tasks-api-openapi.yml
  format: yaml
  label: Mark43 Tasks API
  slug: mark43-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-tasks-api-openapi.yml
- filename: mark43-users-api-openapi.yml
  format: yaml
  label: Mark43 Users API
  slug: mark43-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-users-api-openapi.yml
- filename: mark43-vehicles-api-openapi.yml
  format: yaml
  label: Mark43 Vehicles API
  slug: mark43-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-vehicles-api-openapi.yml
- filename: mark43-warrants-api-openapi.yml
  format: yaml
  label: Mark43 Warrants API
  slug: mark43-warrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-warrants-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mark43 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mark43 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mark43
provider_slug: mark43
scheme_count: 1
schemes:
- description: Secure API token presented via the standard HTTP Basic Authorization header on every request; issued by your Mark43 Technical Services Representative.
  name: httpBasic
  scheme: basic
  sources:
  - openapi/mark43-partnerships-openapi.yml
  type: http
slug: mark43-authentication
source_filename: mark43-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mark43-partnerships-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: httpBasic\n  type: http\n  scheme: basic\n  description: Secure API token presented via the standard HTTP Basic Authorization header on\n    every request; issued by your Mark43 Technical Services Representative.\n  sources:\n  - openapi/mark43-partnerships-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/authentication/mark43-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Public Safety
- Law Enforcement
- Records Management
- Computer-Aided Dispatch
- CAD
- RMS
- GovTech
- Evidence Management
- Government
---
