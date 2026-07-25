---
api_key_in: []
api_specs:
- filename: td-synnex-authentication-api-openapi.yml
  format: yaml
  label: TD SYNNEX Authentication API
  slug: td-synnex-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-authentication-api-openapi.yml
- filename: td-synnex-cart-items-api-openapi.yml
  format: yaml
  label: TD SYNNEX Cart Items API
  slug: td-synnex-cart-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-cart-items-api-openapi.yml
- filename: td-synnex-carts-api-openapi.yml
  format: yaml
  label: TD SYNNEX Carts API
  slug: td-synnex-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-carts-api-openapi.yml
- filename: td-synnex-cloud-providers-api-openapi.yml
  format: yaml
  label: TD SYNNEX Cloud Providers API
  slug: td-synnex-cloud-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-cloud-providers-api-openapi.yml
- filename: td-synnex-customers-api-openapi.yml
  format: yaml
  label: TD SYNNEX Customers API
  slug: td-synnex-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-customers-api-openapi.yml
- filename: td-synnex-orders-api-openapi.yml
  format: yaml
  label: TD SYNNEX Orders API
  slug: td-synnex-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-orders-api-openapi.yml
- filename: td-synnex-products-api-openapi.yml
  format: yaml
  label: TD SYNNEX Products API
  slug: td-synnex-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-products-api-openapi.yml
- filename: td-synnex-provisioning-api-openapi.yml
  format: yaml
  label: TD SYNNEX Provisioning API
  slug: td-synnex-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-provisioning-api-openapi.yml
- filename: td-synnex-reports-api-openapi.yml
  format: yaml
  label: TD SYNNEX Reports API
  slug: td-synnex-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-reports-api-openapi.yml
- filename: td-synnex-subscriptions-api-openapi.yml
  format: yaml
  label: TD SYNNEX Subscriptions API
  slug: td-synnex-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-subscriptions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Td Synnex Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: TD SYNNEX secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: TD SYNNEX
provider_slug: td-synnex
scheme_count: 1
schemes:
- description: TD SYNNEX StreamOne Ion uses OAuth 2.0 with refresh token flow
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://ion.tdsynnex.com/oauth/token
  name: OAuth2
  sources:
  - openapi/td-synnex-streamone-ion-openapi.yml
  type: oauth2
slug: td-synnex-authentication
source_filename: td-synnex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/td-synnex-streamone-ion-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://ion.tdsynnex.com/oauth/token\n    scopes: 2\n  description: TD SYNNEX StreamOne Ion uses OAuth 2.0 with refresh token flow\n  sources:\n  - openapi/td-synnex-streamone-ion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/authentication/td-synnex-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Technology Distribution
- IT Distribution
- Cloud
- Reseller
- StreamOne
- Fortune 100
- B2B
---
