---
api_key_in:
- cookie
api_specs:
- filename: sap-business-one-openapi.yml
  format: yaml
  label: SAP Business One Service Layer API
  slug: service-layer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-business-one/refs/heads/main/openapi/sap-business-one-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sap Business One Authentication
name_suffix: Authentication
oauth_flows: []
overview: SAP Business One secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SAP Business One
provider_slug: sap-business-one
scheme_count: 1
schemes:
- description: Session cookie returned from POST /Login.
  in: cookie
  name: sessionCookie
  parameter: B1SESSION
  sources:
  - openapi/sap-business-one-openapi.yml
  type: apiKey
slug: sap-business-one-authentication
source_filename: sap-business-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-business-one-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: B1SESSION\n  description: Session cookie returned from POST /Login.\n  sources:\n  - openapi/sap-business-one-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-business-one/refs/heads/main/authentication/sap-business-one-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- ERP
- Enterprise Resource Planning
- Accounting
- Inventory Management
- CRM
- Small Business
- Midsize Business
- SAP
---
