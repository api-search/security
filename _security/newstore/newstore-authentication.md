---
api_key_in: []
api_specs:
- filename: newstore-api-openapi-original.json
  format: json
  label: NewStore Omnichannel API
  slug: newstore-omnichannel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newstore/refs/heads/main/openapi/newstore-api-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Newstore Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Newstore secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Newstore
provider_slug: newstore
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 29
    tokenUrl: https://id.p.newstore.net/auth/realms/dodici-demo/protocol/openid-connect/token
  name: oauth
  sources:
  - openapi/newstore-api-openapi-original.json
  type: oauth2
slug: newstore-authentication
source_filename: newstore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/newstore-api-openapi-original.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://id.p.newstore.net/auth/realms/dodici-demo/protocol/openid-connect/token\n    scopes: 29\n  sources:\n  - openapi/newstore-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newstore/refs/heads/main/authentication/newstore-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Retail
- Omnichannel
- Order Management
- Point of Sale
- Ecommerce
- Fulfillment
- Inventory
- Store Operations
- REST
---
