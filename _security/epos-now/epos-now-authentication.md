---
api_key_in: []
api_specs:
- filename: epos-now-openapi.yml
  format: yaml
  label: Epos Now Products API
  slug: epos-now-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epos-now/refs/heads/main/openapi/epos-now-openapi.yml
- filename: epos-now-openapi.yml
  format: yaml
  label: Epos Now Categories API
  slug: epos-now-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epos-now/refs/heads/main/openapi/epos-now-openapi.yml
- filename: epos-now-openapi.yml
  format: yaml
  label: Epos Now Transactions API
  slug: epos-now-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epos-now/refs/heads/main/openapi/epos-now-openapi.yml
- filename: epos-now-openapi.yml
  format: yaml
  label: Epos Now Customers API
  slug: epos-now-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epos-now/refs/heads/main/openapi/epos-now-openapi.yml
- filename: epos-now-openapi.yml
  format: yaml
  label: Epos Now Stock API
  slug: epos-now-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epos-now/refs/heads/main/openapi/epos-now-openapi.yml
- filename: epos-now-openapi.yml
  format: yaml
  label: Epos Now Devices and Webhooks API
  slug: epos-now-devices-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epos-now/refs/heads/main/openapi/epos-now-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Epos Now Authentication
name_suffix: Authentication
oauth_flows: []
overview: Epos Now secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Epos Now
provider_slug: epos-now
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication. The access token is the Base64 encoding of the string "API Key:API Secret" (the API Key, a colon character, then the API Secret, with no spaces). It is sent as the header "Authorization: Basic {token}", alongside a Content-Type header such as application/json. Credentials are issued per API Device registered under Web Integrations in the Epos Now Back Office; each device has its own key/secret pair and can be regenerated, and the token differs for every registered device.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/epos-now-openapi.yml
  - https://developer.eposnowhq.com/Docs/Authentication
  - https://developer.eposnowhq.com/Setup/ApiDevice
  type: http
slug: epos-now-authentication
source_filename: epos-now-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/epos-now-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication. The access token is the Base64 encoding of the\n    string \"API Key:API Secret\" (the API Key, a colon character, then the API\n    Secret, with no spaces). It is sent as the header\n    \"Authorization: Basic {token}\", alongside a Content-Type header such as\n    application/json. Credentials are issued per API Device registered under\n    Web Integrations in the Epos Now Back Office; each device has its own\n    key/secret pair and can be regenerated, and the token differs for every\n    registered device.\n  sources:\n  - openapi/epos-now-openapi.yml\n  - https://developer.eposnowhq.com/Docs/Authentication\n  - https://developer.eposnowhq.com/Setup/ApiDevice\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epos-now/refs/heads/main/authentication/epos-now-authentication.yml
summary_line: http · 1 scheme
tags:
- Point of Sale
- POS
- Retail
- Hospitality
- Payments
- Inventory
- Commerce
- Ecommerce
---
