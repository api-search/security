---
api_key_in: []
api_specs:
- filename: toast-tab-authentication-openapi.yml
  format: yaml
  label: Toast Authentication API
  slug: toast-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-authentication-openapi.yml
- filename: toast-tab-restaurants-openapi.yml
  format: yaml
  label: Toast Restaurants API
  slug: toast-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-restaurants-openapi.yml
- filename: toast-tab-menus-openapi.yml
  format: yaml
  label: Toast Menus API (V2)
  slug: toast-menus-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-menus-openapi.yml
- filename: toast-tab-orders-openapi.yml
  format: yaml
  label: Toast Orders API
  slug: toast-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-orders-openapi.yml
- filename: toast-tab-labor-openapi.yml
  format: yaml
  label: Toast Labor API
  slug: toast-labor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-labor-openapi.yml
- filename: toast-tab-stock-openapi.yml
  format: yaml
  label: Toast Stock API
  slug: toast-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-stock-openapi.yml
- filename: toast-tab-partners-openapi.yml
  format: yaml
  label: Toast Partners API
  slug: toast-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-partners-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Toast Tab Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Toast secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Toast
provider_slug: toast-tab
scheme_count: 1
schemes:
- description: "Access to Toast APIs, specific endpoints, \nand specific API endpoint operations is \ncontrolled by the scopes that are associated \nwith your API account. \nA full reference for Toast API scopes and \ntheir capabilities can be found in the\n[_Toast Developer Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html)."
  flows:
  - flow: clientCredentials
    scopes: 7
    tokenUrl: https://toast-api-server/authentication/v1/authentication/login
  name: oauth2
  sources:
  - openapi/toast-tab-labor-openapi.yml
  - openapi/toast-tab-menus-openapi.yml
  - openapi/toast-tab-orders-openapi.yml
  - openapi/toast-tab-partners-openapi.yml
  - openapi/toast-tab-restaurants-openapi.yml
  - openapi/toast-tab-stock-openapi.yml
  type: oauth2
slug: toast-tab-authentication
source_filename: toast-tab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/toast-tab-labor-openapi.yml, openapi/toast-tab-menus-openapi.yml, openapi/toast-tab-orders-openapi.yml,\n  openapi/toast-tab-partners-openapi.yml, openapi/toast-tab-restaurants-openapi.yml, openapi/toast-tab-stock-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://toast-api-server/authentication/v1/authentication/login\n    scopes: 7\n  description: \"Access to Toast APIs, specific endpoints, \\nand specific API endpoint operations\\\n    \\ is \\ncontrolled by the scopes that are associated \\nwith your API account. \\nA full reference\\\n    \\ for Toast API scopes and \\ntheir capabilities can be found in the\\n[_Toast Developer Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html).\"\n  sources:\n  - openapi/toast-tab-labor-openapi.yml\n  - openapi/toast-tab-menus-openapi.yml\n\
  \  - openapi/toast-tab-orders-openapi.yml\n  - openapi/toast-tab-partners-openapi.yml\n  - openapi/toast-tab-restaurants-openapi.yml\n  - openapi/toast-tab-stock-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/authentication/toast-tab-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Restaurants
- Point Of Sale
- Payments
- Online Ordering
- Delivery
- Loyalty
- Gift Cards
- Menus
- Orders
- Kitchen
- Labor
- Scheduling
- Inventory
- Hospitality
- Partner Integrations
---
