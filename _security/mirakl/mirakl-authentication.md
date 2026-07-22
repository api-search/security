---
api_key_in:
- header
api_specs:
- filename: mirakl-mmp-seller-openapi.json
  format: json
  label: Mirakl Marketplace Platform — Seller API
  slug: mirakl-marketplace-platform-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mmp-seller-openapi.json
- filename: mirakl-mmp-operator-openapi.json
  format: json
  label: Mirakl Marketplace Platform — Operator API
  slug: mirakl-marketplace-platform-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mmp-operator-openapi.json
- filename: mirakl-mms-seller-openapi.json
  format: json
  label: Mirakl Platform for Services — Seller API
  slug: mirakl-platform-for-services-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mms-seller-openapi.json
- filename: mirakl-mms-operator-openapi.json
  format: json
  label: Mirakl Platform for Services — Operator API
  slug: mirakl-platform-for-services-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mms-operator-openapi.json
- filename: mirakl-mcm-seller-openapi.json
  format: json
  label: Mirakl Catalog Manager — Seller API
  slug: mirakl-catalog-manager-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mcm-seller-openapi.json
- filename: mirakl-mcm-operator-openapi.json
  format: json
  label: Mirakl Catalog Manager — Operator API
  slug: mirakl-catalog-manager-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mcm-operator-openapi.json
- filename: mirakl-connect-channel-openapi.json
  format: json
  label: Mirakl Connect Channel Platform API
  slug: mirakl-connect-channel-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-connect-channel-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Mirakl Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Mirakl secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Mirakl
provider_slug: mirakl
scheme_count: 3
schemes:
- description: For more information, see our [Authentication System documentation](https://help.mirakl.com/docs/customers/page/topics/Mirakl/partners_integration/authentication_system.htm)
  flows:
  - authorizationUrl: https://auth.mirakl.net/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://auth.mirakl.net/oauth/token
  name: OAuth-2
  sources:
  - openapi/mirakl-mcm-operator-openapi.json
  - openapi/mirakl-mmp-operator-openapi.json
  - openapi/mirakl-mms-operator-openapi.json
  type: oauth2
- bearerFormat: JWT
  name: Operator-Bearer-Token
  scheme: bearer
  sources:
  - openapi/mirakl-mcm-operator-openapi.json
  - openapi/mirakl-mmp-operator-openapi.json
  - openapi/mirakl-mms-operator-openapi.json
  type: http
- in: header
  name: Shop-API-Key
  parameter: Authorization
  sources:
  - openapi/mirakl-mcm-seller-openapi.json
  - openapi/mirakl-mmp-seller-openapi.json
  - openapi/mirakl-mms-operator-openapi.json
  - openapi/mirakl-mms-seller-openapi.json
  type: apiKey
slug: mirakl-authentication
source_filename: mirakl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mirakl-mcm-operator-openapi.json, openapi/mirakl-mcm-seller-openapi.json, openapi/mirakl-mmp-operator-openapi.json,\n  openapi/mirakl-mmp-seller-openapi.json, openapi/mirakl-mms-operator-openapi.json, openapi/mirakl-mms-seller-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth-2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.mirakl.net/authorize\n    tokenUrl: https://auth.mirakl.net/oauth/token\n    scopes: 0\n  description: For more information, see our [Authentication System documentation](https://help.mirakl.com/docs/customers/page/topics/Mirakl/partners_integration/authentication_system.htm)\n  sources:\n  - openapi/mirakl-mcm-operator-openapi.json\n  - openapi/mirakl-mmp-operator-openapi.json\n  - openapi/mirakl-mms-operator-openapi.json\n- name: Operator-Bearer-Token\n\
  \  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/mirakl-mcm-operator-openapi.json\n  - openapi/mirakl-mmp-operator-openapi.json\n  - openapi/mirakl-mms-operator-openapi.json\n- name: Shop-API-Key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/mirakl-mcm-seller-openapi.json\n  - openapi/mirakl-mmp-seller-openapi.json\n  - openapi/mirakl-mms-operator-openapi.json\n  - openapi/mirakl-mms-seller-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/authentication/mirakl-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Commerce
- eCommerce
- Marketplace
- Dropship
- Retail
- Catalog
- Orders
- Retail Media
- B2B
---
