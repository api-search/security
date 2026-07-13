---
api_key_in: []
api_specs:
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Team Members
  slug: team-members
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Leave / Absences
  slug: leave-absences
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Leave Allowances
  slug: leave-allowances
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Company
  slug: company
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Charliehr Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CharlieHR secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CharlieHR
provider_slug: charliehr
scheme_count: 1
schemes:
- description: OAuth 2.0. A Client ID and Client Secret issued in the CharlieHR app are exchanged for an access token, which is sent in the Authorization header of each request.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://charliehr.com/oauth/token
  name: oauth2
  sources:
  - openapi/charliehr-openapi.yml
  type: oauth2
slug: charliehr-authentication
source_filename: charliehr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/charliehr-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://charliehr.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0. A Client ID and Client Secret issued in the CharlieHR app are exchanged\n    for an access token, which is sent in the Authorization header of each request.\n  sources:\n  - openapi/charliehr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/authentication/charliehr-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- HR
- HRIS
- People
- Leave
- Time Off
---
