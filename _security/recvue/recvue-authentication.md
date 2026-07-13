---
api_key_in: []
api_specs:
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Revenue Recognition API
  slug: recvue-revenue-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Billing API
  slug: recvue-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Billing Schedules API
  slug: recvue-billing-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Orders API
  slug: recvue-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Usage and Deliveries API
  slug: recvue-usage-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Pricing API
  slug: recvue-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Customers and Accounts API
  slug: recvue-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
- filename: recvue-openapi.yml
  format: yaml
  label: RecVue Invoices and Adjustments API
  slug: recvue-invoices-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/openapi/recvue-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: sourced
name: Recvue Authentication
name_suffix: Authentication
oauth_flows: []
overview: RecVue secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RecVue
provider_slug: recvue
scheme_count: 1
schemes:
- description: RecVue authenticates with OAuth2 using the client_credentials grant. Request an access token from the token endpoint by sending grant_type=client_credentials with a Basic auth header (client_id:client_secret) or client_id/client_secret as x-www-form-urlencoded form params. The returned access token is passed as an Authorization Bearer header on subsequent API calls. Sandbox uses host sandbox-api.recvue.com.
  flow: clientCredentials
  grantType: client_credentials
  name: oauth2ClientCredentials
  sources:
  - https://developer.recvue.com/reference/tokenusingpost
  tokenUrl: https://api.recvue.com/api/v2.0/api/scim/oauth/token
  type: oauth2
slug: recvue-authentication
source_filename: recvue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: sourced\nsource: https://developer.recvue.com/reference/tokenusingpost\nsummary:\n  types:\n  - oauth2\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://api.recvue.com/api/v2.0/api/scim/oauth/token\n  grantType: client_credentials\n  description: >-\n    RecVue authenticates with OAuth2 using the client_credentials grant.\n    Request an access token from the token endpoint by sending\n    grant_type=client_credentials with a Basic auth header (client_id:client_secret)\n    or client_id/client_secret as x-www-form-urlencoded form params. The\n    returned access token is passed as an Authorization Bearer header on\n    subsequent API calls. Sandbox uses host sandbox-api.recvue.com.\n  sources:\n  - https://developer.recvue.com/reference/tokenusingpost\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recvue/refs/heads/main/authentication/recvue-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Revenue Recognition
- ASC 606
- Billing
- Order-to-Cash
- Revenue Management
- Usage-Based Billing
- Partner Settlements
- IFRS 15
- Subscription Billing
- Enterprise
---
