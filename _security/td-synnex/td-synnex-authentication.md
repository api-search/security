---
api_key_in: []
api_specs:
- filename: td-synnex-streamone-ion-openapi.yml
  format: yaml
  label: TD SYNNEX StreamOne Ion API
  slug: streamone-ion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-streamone-ion-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Td Synnex Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: TD SYNNEX secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: TD SYNNEX
provider_slug: td-synnex
scheme_count: 1
schemes:
- description: TD SYNNEX StreamOne Ion uses OAuth 2.0 with refresh token flow
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://ion.tdsynnex.com/oauth/token
  name: OAuth2
  sources:
  - openapi/td-synnex-streamone-ion-openapi.yml
  type: oauth2
slug: td-synnex-authentication
source_filename: td-synnex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/td-synnex-streamone-ion-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://ion.tdsynnex.com/oauth/token\n    scopes: 2\n  description: TD SYNNEX StreamOne Ion uses OAuth 2.0 with refresh token flow\n  sources:\n  - openapi/td-synnex-streamone-ion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/authentication/td-synnex-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Technology Distribution
- IT Distribution
- Cloud
- Reseller
- StreamOne
- Fortune 100
- B2B
---
