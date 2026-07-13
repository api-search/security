---
api_key_in: []
api_specs:
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Clients API
  slug: repsly-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Representatives API
  slug: repsly-representatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Visits API
  slug: repsly-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Products API
  slug: repsly-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Forms API
  slug: repsly-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Photos API
  slug: repsly-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Pricelists API
  slug: repsly-pricelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Purchase Orders API
  slug: repsly-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Import and Export API
  slug: repsly-import-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Repsly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Repsly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Repsly
provider_slug: repsly
scheme_count: 1
schemes:
- description: HTTP Basic authentication over SSL. Use the API username and password from the Repsly settings page (API Settings) - these differ from your Repsly login credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/repsly-openapi.yml
  type: http
slug: repsly-authentication
source_filename: repsly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/repsly-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication over SSL. Use the API username and password from the\n    Repsly settings page (API Settings) - these differ from your Repsly login credentials.\n  sources:\n  - openapi/repsly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/authentication/repsly-authentication.yml
summary_line: http · 1 scheme
tags:
- Retail Execution
- Field Sales
- Merchandising
- CPG
- Retail Audits
- Sales Force Automation
---
