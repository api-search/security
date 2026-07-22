---
api_key_in: []
api_specs:
- filename: simplivity-omnistack-openapi-original.json
  format: json
  label: HPE OmniStack REST API
  slug: hpe-omnistack-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-omnistack-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Simplivity Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: SimpliVity secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: SimpliVity
provider_slug: simplivity
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 2
    tokenUrl: /oauth/token
  name: OAuth2
  sources:
  - openapi/simplivity-omnistack-openapi-original.json
  type: oauth2
slug: simplivity-authentication
source_filename: simplivity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/simplivity-omnistack-openapi-original.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /oauth/token\n    scopes: 2\n  sources:\n  - openapi/simplivity-omnistack-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/authentication/simplivity-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Big Data
- Hyperconverged Infrastructure
- Virtualization
- Backup
- Disaster Recovery
- Data Center
- Storage
- Cloud Infrastructure
- HPE
---
