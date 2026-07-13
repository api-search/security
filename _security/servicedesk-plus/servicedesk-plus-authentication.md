---
api_key_in: []
api_specs:
- filename: servicedesk-plus-openapi.yml
  format: yaml
  label: ServiceDesk Plus REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicedesk-plus/refs/heads/main/openapi/servicedesk-plus-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Servicedesk Plus Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ManageEngine ServiceDesk Plus secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ManageEngine ServiceDesk Plus
provider_slug: servicedesk-plus
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: oauth2
  sources:
  - openapi/servicedesk-plus-openapi.yml
  type: oauth2
slug: servicedesk-plus-authentication
source_filename: servicedesk-plus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/servicedesk-plus-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n    scopes: 5\n  sources:\n  - openapi/servicedesk-plus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicedesk-plus/refs/heads/main/authentication/servicedesk-plus-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- ITSM
- Help Desk
- Incident Management
- Asset Management
- CMDB
---
