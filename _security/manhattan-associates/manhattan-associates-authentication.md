---
api_key_in: []
api_specs:
- filename: manhattan-associates-omni-openapi.yml
  format: yaml
  label: Manhattan Active Omni and Enterprise Promise & Fulfill API
  slug: manhattan-active-omni-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manhattan-associates/refs/heads/main/openapi/manhattan-associates-omni-openapi.yml
- filename: manhattan-associates-wms-openapi.yml
  format: yaml
  label: Manhattan Active Supply Chain API
  slug: manhattan-active-supply-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manhattan-associates/refs/heads/main/openapi/manhattan-associates-wms-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Manhattan Associates Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: manhattan-associates secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: manhattan-associates
provider_slug: manhattan-associates
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://auth.developer.manh.com/oauth2/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/manhattan-associates-omni-openapi.yml
  - openapi/manhattan-associates-wms-openapi.yml
  type: oauth2
slug: manhattan-associates-authentication
source_filename: manhattan-associates-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/manhattan-associates-omni-openapi.yml, openapi/manhattan-associates-wms-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.developer.manh.com/oauth2/token\n    scopes: 3\n  sources:\n  - openapi/manhattan-associates-omni-openapi.yml\n  - openapi/manhattan-associates-wms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manhattan-associates/refs/heads/main/authentication/manhattan-associates-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
