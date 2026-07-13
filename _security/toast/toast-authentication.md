---
api_key_in: []
api_specs:
- filename: toast-orders-openapi.yaml
  format: yaml
  label: Toast Orders API
  slug: toast-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-orders-openapi.yaml
- filename: toast-menus-openapi.yaml
  format: yaml
  label: Toast Menus API
  slug: toast-menus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-menus-openapi.yaml
- filename: toast-labor-openapi.yaml
  format: yaml
  label: Toast Labor API
  slug: toast-labor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-labor-openapi.yaml
- filename: toast-restaurants-openapi.yaml
  format: yaml
  label: Toast Restaurants API
  slug: toast-restaurants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-restaurants-openapi.yaml
- filename: toast-stock-openapi.yaml
  format: yaml
  label: Toast Stock API
  slug: toast-stock
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-stock-openapi.yaml
- filename: toast-partners-openapi.yaml
  format: yaml
  label: Toast Partners API
  slug: toast-partners
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-partners-openapi.yaml
- filename: toast-authentication-openapi.yaml
  format: yaml
  label: Toast Authentication API
  slug: toast-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-authentication-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Toast Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Toast secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Toast
provider_slug: toast
scheme_count: 1
schemes:
- description: "Access to Toast APIs, specific endpoints, \nand specific API endpoint operations is \ncontrolled by the scopes that are associated \nwith your API account. \nA full reference for Toast API scopes and \ntheir capabilities can be found in the\n[_Toast Developer Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html)."
  flows:
  - flow: clientCredentials
    scopes: 7
    tokenUrl: https://toast-api-server/authentication/v1/authentication/login
  name: oauth2
  sources:
  - openapi/toast-labor-openapi.yaml
  - openapi/toast-menus-openapi.yaml
  - openapi/toast-orders-openapi.yaml
  - openapi/toast-partners-openapi.yaml
  - openapi/toast-restaurants-openapi.yaml
  - openapi/toast-stock-openapi.yaml
  type: oauth2
slug: toast-authentication
source_filename: toast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/toast-labor-openapi.yaml, openapi/toast-menus-openapi.yaml, openapi/toast-orders-openapi.yaml,\n  openapi/toast-partners-openapi.yaml, openapi/toast-restaurants-openapi.yaml, openapi/toast-stock-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://toast-api-server/authentication/v1/authentication/login\n    scopes: 7\n  description: \"Access to Toast APIs, specific endpoints, \\nand specific API endpoint operations\\\n    \\ is \\ncontrolled by the scopes that are associated \\nwith your API account. \\nA full reference\\\n    \\ for Toast API scopes and \\ntheir capabilities can be found in the\\n[_Toast Developer Guide_](https://doc.toasttab.com/doc/devguide/apiScopes.html).\"\n  sources:\n  - openapi/toast-labor-openapi.yaml\n  - openapi/toast-menus-openapi.yaml\n  - openapi/toast-orders-openapi.yaml\n\
  \  - openapi/toast-partners-openapi.yaml\n  - openapi/toast-restaurants-openapi.yaml\n  - openapi/toast-stock-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/authentication/toast-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Food Service
- Point of Sale
- Restaurants
- Hospitality
---
