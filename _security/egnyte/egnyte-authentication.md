---
api_key_in: []
api_specs:
- filename: egnyte-openapi.yml
  format: yaml
  label: Egnyte Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egnyte/refs/heads/main/openapi/egnyte-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Egnyte Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Egnyte secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Egnyte
provider_slug: egnyte
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://{domain}.egnyte.com/puboauth/token
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://{domain}.egnyte.com/puboauth/token
  name: oauth2
  sources:
  - openapi/egnyte-openapi.yml
  type: oauth2
slug: egnyte-authentication
source_filename: egnyte-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/egnyte-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{domain}.egnyte.com/puboauth/token\n    tokenUrl: https://{domain}.egnyte.com/puboauth/token\n    scopes: 6\n  sources:\n  - openapi/egnyte-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/egnyte/refs/heads/main/authentication/egnyte-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- File Sharing
- Content Collaboration
- Enterprise Storage
- Document Management
- Governance
- Data Security
---
