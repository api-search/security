---
api_key_in: []
api_specs:
- filename: toast-authentication-api-openapi.yml
  format: yaml
  label: Toast Authentication API
  slug: toast-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-authentication-api-openapi.yml
- filename: toast-connectedrestaurants-api-openapi.yml
  format: yaml
  label: Toast ConnectedRestaurants API
  slug: toast-connectedrestaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-connectedrestaurants-api-openapi.yml
- filename: toast-discounts-api-openapi.yml
  format: yaml
  label: Toast Discounts API
  slug: toast-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-discounts-api-openapi.yml
- filename: toast-employees-api-openapi.yml
  format: yaml
  label: Toast Employees API
  slug: toast-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-employees-api-openapi.yml
- filename: toast-groups-api-openapi.yml
  format: yaml
  label: Toast Groups API
  slug: toast-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-groups-api-openapi.yml
- filename: toast-jobs-api-openapi.yml
  format: yaml
  label: Toast Jobs API
  slug: toast-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-jobs-api-openapi.yml
- filename: toast-menus-api-openapi.yml
  format: yaml
  label: Toast Menus API
  slug: toast-menus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-menus-api-openapi.yml
- filename: toast-metadata-api-openapi.yml
  format: yaml
  label: Toast Metadata API
  slug: toast-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-metadata-api-openapi.yml
- filename: toast-orders-api-openapi.yml
  format: yaml
  label: Toast Orders API
  slug: toast-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-orders-api-openapi.yml
- filename: toast-payments-api-openapi.yml
  format: yaml
  label: Toast Payments API
  slug: toast-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-payments-api-openapi.yml
- filename: toast-restaurants-api-openapi.yml
  format: yaml
  label: Toast Restaurants API
  slug: toast-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-restaurants-api-openapi.yml
- filename: toast-shifts-api-openapi.yml
  format: yaml
  label: Toast Shifts API
  slug: toast-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-shifts-api-openapi.yml
- filename: toast-stock-api-openapi.yml
  format: yaml
  label: Toast Stock API
  slug: toast-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-stock-api-openapi.yml
- filename: toast-time-entries-api-openapi.yml
  format: yaml
  label: Toast Time entries API
  slug: toast-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-time-entries-api-openapi.yml
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
