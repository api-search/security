---
api_key_in: []
api_specs:
- filename: swagger.json
  format: json
  label: EVE Swagger Interface (ESI)
  slug: eve-swagger-interface
  spec_type: OpenAPI
  url: https://esi.evetech.net/latest/swagger.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Eve Online Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: EVE Online secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: EVE Online
provider_slug: eve-online
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.eveonline.com/v2/oauth/authorize
    flow: implicit
    scopes: 63
  name: evesso
  sources:
  - openapi/eve-online-openapi.yml
  type: oauth2
slug: eve-online-authentication
source_filename: eve-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eve-online-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: evesso\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.eveonline.com/v2/oauth/authorize\n    scopes: 63\n  sources:\n  - openapi/eve-online-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eve-online/refs/heads/main/authentication/eve-online-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Authentication
- Authorization
- Gaming
- Images
- MMO
- OAuth2
- REST
- SSO
- Static Data
---
