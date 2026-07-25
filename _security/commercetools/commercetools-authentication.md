---
api_key_in: []
api_specs:
- filename: commercetools-carts-api-openapi.yml
  format: yaml
  label: commercetools Carts API
  slug: commercetools-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-carts-api-openapi.yml
- filename: commercetools-categories-api-openapi.yml
  format: yaml
  label: commercetools Categories API
  slug: commercetools-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-categories-api-openapi.yml
- filename: commercetools-changehistory-api-openapi.yml
  format: yaml
  label: commercetools ChangeHistory API
  slug: commercetools-changehistory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-changehistory-api-openapi.yml
- filename: commercetools-customers-api-openapi.yml
  format: yaml
  label: commercetools Customers API
  slug: commercetools-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-customers-api-openapi.yml
- filename: commercetools-importcontainers-api-openapi.yml
  format: yaml
  label: commercetools ImportContainers API
  slug: commercetools-importcontainers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-importcontainers-api-openapi.yml
- filename: commercetools-importoperations-api-openapi.yml
  format: yaml
  label: commercetools ImportOperations API
  slug: commercetools-importoperations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-importoperations-api-openapi.yml
- filename: commercetools-inventory-api-openapi.yml
  format: yaml
  label: commercetools Inventory API
  slug: commercetools-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-inventory-api-openapi.yml
- filename: commercetools-orders-api-openapi.yml
  format: yaml
  label: commercetools Orders API
  slug: commercetools-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-orders-api-openapi.yml
- filename: commercetools-payments-api-openapi.yml
  format: yaml
  label: commercetools Payments API
  slug: commercetools-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-payments-api-openapi.yml
- filename: commercetools-products-api-openapi.yml
  format: yaml
  label: commercetools Products API
  slug: commercetools-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-products-api-openapi.yml
- filename: commercetools-productvariants-api-openapi.yml
  format: yaml
  label: commercetools ProductVariants API
  slug: commercetools-productvariants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-productvariants-api-openapi.yml
- filename: commercetools-project-api-openapi.yml
  format: yaml
  label: commercetools Project API
  slug: commercetools-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-project-api-openapi.yml
- filename: commercetools-standaloneprices-api-openapi.yml
  format: yaml
  label: commercetools StandalonePrices API
  slug: commercetools-standaloneprices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-standaloneprices-api-openapi.yml
- filename: commercetools-subscriptions-api-openapi.yml
  format: yaml
  label: commercetools Subscriptions API
  slug: commercetools-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-subscriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Commercetools Authentication
name_suffix: Authentication
oauth_flows: []
overview: commercetools secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: commercetools
provider_slug: commercetools
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token obtained from the commercetools authentication service using client credentials flow. Requires the view_audit_log scope.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/commercetools-change-history-api-openapi.yml
  - openapi/commercetools-http-api-openapi.yml
  - openapi/commercetools-import-api-openapi.yml
  type: http
slug: commercetools-authentication
source_filename: commercetools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/commercetools-change-history-api-openapi.yml, openapi/commercetools-http-api-openapi.yml,\n  openapi/commercetools-import-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token obtained from the commercetools authentication service\n    using client credentials flow. Requires the view_audit_log scope.\n  sources:\n  - openapi/commercetools-change-history-api-openapi.yml\n  - openapi/commercetools-http-api-openapi.yml\n  - openapi/commercetools-import-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/authentication/commercetools-authentication.yml
summary_line: http · 1 scheme
tags:
- Commerce
- Composable Commerce
- E-Commerce
- GraphQL
- REST
- SDK
---
