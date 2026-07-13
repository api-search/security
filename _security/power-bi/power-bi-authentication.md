---
api_key_in: []
api_specs:
- filename: powerbi.json
  format: json
  label: Power BI REST API
  slug: power-bi-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/powerbi/data-plane/Microsoft.PowerBI/stable/v1.0/powerbi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Power Bi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Power BI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Power BI
provider_slug: power-bi
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Azure Active Directory OAuth 2.0 access token. Obtain a token by registering an Azure AD application and requesting the Power BI Service scope (https://analysis.windows.net/powerbi/api/.default).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/power-bi-rest-api-openapi.yml
  type: http
slug: power-bi-authentication
source_filename: power-bi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/power-bi-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Azure Active Directory OAuth 2.0 access token. Obtain a token by registering\n    an Azure AD application and requesting the Power BI Service scope (https://analysis.windows.net/powerbi/api/.default).\n  sources:\n  - openapi/power-bi-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/authentication/power-bi-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
---
