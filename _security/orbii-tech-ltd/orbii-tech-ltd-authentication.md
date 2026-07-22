---
api_key_in: []
api_specs:
- filename: orbii-tech-ltd-main-openapi.json
  format: json
  label: Orbii API
  slug: orbii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii-tech-ltd/refs/heads/main/openapi/orbii-tech-ltd-main-openapi.json
- filename: orbii-tech-ltd-ksa-openapi.json
  format: json
  label: Orbii KSA API
  slug: orbii-ksa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii-tech-ltd/refs/heads/main/openapi/orbii-tech-ltd-ksa-openapi.json
- filename: orbii-tech-ltd-omn-openapi.json
  format: json
  label: Orbii OMN API
  slug: orbii-omn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii-tech-ltd/refs/heads/main/openapi/orbii-tech-ltd-omn-openapi.json
- filename: orbii-tech-ltd-foodics-openapi.json
  format: json
  label: Orbii API - Foodics
  slug: orbii-api-foodics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii-tech-ltd/refs/heads/main/openapi/orbii-tech-ltd-foodics-openapi.json
- filename: orbii-tech-ltd-rewaa-openapi.json
  format: json
  label: Orbii API - Rewaa
  slug: orbii-api-rewaa
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii-tech-ltd/refs/heads/main/openapi/orbii-tech-ltd-rewaa-openapi.json
auth_types:
- credentials-query
description: ''
kind: authentication
layout: security
method: derived
name: Orbii Tech Ltd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orbii Tech Ltd secures its APIs with credentials-query across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orbii Tech Ltd
provider_slug: orbii-tech-ltd
scheme_count: 1
schemes:
- applied_to: per-operation (not global)
  in: query
  name: query-credentials
  parameters:
  - user
  - password
  sources:
  - orbii-tech-ltd-foodics-openapi.json
  - orbii-tech-ltd-ksa-openapi.json
  - orbii-tech-ltd-main-openapi.json
  - orbii-tech-ltd-omn-openapi.json
  type: apiKey-like
slug: orbii-tech-ltd-authentication
source_filename: orbii-tech-ltd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/ (query parameters)\nsummary:\n  types:\n  - credentials-query\n  note: The published OpenAPI declares no components.securitySchemes and no global security. Operations\n    authenticate by passing user and password as query-string parameters. Credentials in query strings\n    are logged by proxies/servers and are not a recommended pattern; captured here as the provider publishes\n    it.\nschemes:\n- name: query-credentials\n  type: apiKey-like\n  in: query\n  parameters:\n  - user\n  - password\n  applied_to: per-operation (not global)\n  sources:\n  - orbii-tech-ltd-foodics-openapi.json\n  - orbii-tech-ltd-ksa-openapi.json\n  - orbii-tech-ltd-main-openapi.json\n  - orbii-tech-ltd-omn-openapi.json\ndocs: https://api.docs.orbii.ai/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbii-tech-ltd/refs/heads/main/authentication/orbii-tech-ltd-authentication.yml
summary_line: credentials-query · 1 scheme
tags:
- Company
- Fintech
- Lending
- Credit Scoring
- Underwriting
- Embedded Finance
- SME Finance
- Risk
- MENA
- Financial Data
---
