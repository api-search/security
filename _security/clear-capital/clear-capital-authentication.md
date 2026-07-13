---
api_key_in: []
api_specs:
- filename: clear-capital-openapi.yml
  format: yaml
  label: Clear Capital ClearAVM / Valuation API
  slug: clearavm-valuation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-capital/refs/heads/main/openapi/clear-capital-openapi.yml
- filename: clear-capital-openapi.yml
  format: yaml
  label: Clear Capital Property Data API
  slug: property-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-capital/refs/heads/main/openapi/clear-capital-openapi.yml
- filename: clear-capital-openapi.yml
  format: yaml
  label: Clear Capital Comparables (Comps) API
  slug: comps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-capital/refs/heads/main/openapi/clear-capital-openapi.yml
- filename: clear-capital-openapi.yml
  format: yaml
  label: Clear Capital Appraisal & Orders API
  slug: appraisal-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-capital/refs/heads/main/openapi/clear-capital-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clear Capital Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clear Capital secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clear Capital
provider_slug: clear-capital
scheme_count: 1
schemes:
- description: System-to-system authentication over encrypted transport, as described in Clear Capital's product documentation. Exact token issuance and header details are documented in the gated developer portal and are not reproduced here.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/clear-capital-openapi.yml
  type: http
slug: clear-capital-authentication
source_filename: clear-capital-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clear-capital-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: System-to-system authentication over encrypted transport, as described in Clear\n    Capital's product documentation. Exact token issuance and header details are documented\n    in the gated developer portal and are not reproduced here.\n  sources:\n  - openapi/clear-capital-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clear-capital/refs/heads/main/authentication/clear-capital-authentication.yml
summary_line: http · 1 scheme
tags:
- Real Estate
- Property Data
- Valuation
- AVM
- Appraisal
- Mortgage
---
