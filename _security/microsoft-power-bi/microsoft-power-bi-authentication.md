---
api_key_in: []
api_specs:
- filename: microsoft-power-bi-apps-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Apps API
  slug: microsoft-power-bi-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-apps-api-openapi.yml
- filename: microsoft-power-bi-capacities-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Capacities API
  slug: microsoft-power-bi-capacities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-capacities-api-openapi.yml
- filename: microsoft-power-bi-dashboards-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Dashboards API
  slug: microsoft-power-bi-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-dashboards-api-openapi.yml
- filename: microsoft-power-bi-dataflows-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Dataflows API
  slug: microsoft-power-bi-dataflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-dataflows-api-openapi.yml
- filename: microsoft-power-bi-datasets-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Datasets API
  slug: microsoft-power-bi-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-datasets-api-openapi.yml
- filename: microsoft-power-bi-embedtoken-api-openapi.yml
  format: yaml
  label: Microsoft Power BI EmbedToken API
  slug: microsoft-power-bi-embedtoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-embedtoken-api-openapi.yml
- filename: microsoft-power-bi-gateways-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Gateways API
  slug: microsoft-power-bi-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-gateways-api-openapi.yml
- filename: microsoft-power-bi-groups-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Groups API
  slug: microsoft-power-bi-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-groups-api-openapi.yml
- filename: microsoft-power-bi-imports-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Imports API
  slug: microsoft-power-bi-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-imports-api-openapi.yml
- filename: microsoft-power-bi-reports-api-openapi.yml
  format: yaml
  label: Microsoft Power BI Reports API
  slug: microsoft-power-bi-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/openapi/microsoft-power-bi-reports-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Power Bi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Power BI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Power BI
provider_slug: microsoft-power-bi
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-power-bi-openapi.yml
  type: http
slug: microsoft-power-bi-authentication
source_filename: microsoft-power-bi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-power-bi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/microsoft-power-bi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-bi/refs/heads/main/authentication/microsoft-power-bi-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Business Intelligence
- Dashboards
- Microsoft
- Reports
---
