---
api_key_in:
- header
api_specs:
- filename: mirakl-carriers-api-openapi.yml
  format: yaml
  label: Mirakl Carriers API
  slug: mirakl-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-carriers-api-openapi.yml
- filename: mirakl-catalog-configuration-api-openapi.yml
  format: yaml
  label: Mirakl Catalog Configuration API
  slug: mirakl-catalog-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-catalog-configuration-api-openapi.yml
- filename: mirakl-incidents-api-openapi.yml
  format: yaml
  label: Mirakl Incidents API
  slug: mirakl-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-incidents-api-openapi.yml
- filename: mirakl-invoicing-and-accounting-api-openapi.yml
  format: yaml
  label: Mirakl Invoicing and Accounting API
  slug: mirakl-invoicing-and-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-invoicing-and-accounting-api-openapi.yml
- filename: mirakl-messages-api-openapi.yml
  format: yaml
  label: Mirakl Messages API
  slug: mirakl-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-messages-api-openapi.yml
- filename: mirakl-multiple-shipments-api-openapi.yml
  format: yaml
  label: Mirakl Multiple shipments API
  slug: mirakl-multiple-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-multiple-shipments-api-openapi.yml
- filename: mirakl-offers-api-openapi.yml
  format: yaml
  label: Mirakl Offers API
  slug: mirakl-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-offers-api-openapi.yml
- filename: mirakl-orders-api-openapi.yml
  format: yaml
  label: Mirakl Orders API
  slug: mirakl-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-orders-api-openapi.yml
- filename: mirakl-picklists-api-openapi.yml
  format: yaml
  label: Mirakl Picklists API
  slug: mirakl-picklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-picklists-api-openapi.yml
- filename: mirakl-platform-settings-api-openapi.yml
  format: yaml
  label: Mirakl Platform Settings API
  slug: mirakl-platform-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-platform-settings-api-openapi.yml
- filename: mirakl-product-feedback-api-openapi.yml
  format: yaml
  label: Mirakl Product Feedback API
  slug: mirakl-product-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-product-feedback-api-openapi.yml
- filename: mirakl-products-api-openapi.yml
  format: yaml
  label: Mirakl Products API
  slug: mirakl-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-products-api-openapi.yml
- filename: mirakl-promotions-api-openapi.yml
  format: yaml
  label: Mirakl Promotions API
  slug: mirakl-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-promotions-api-openapi.yml
- filename: mirakl-returns-api-openapi.yml
  format: yaml
  label: Mirakl Returns API
  slug: mirakl-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-returns-api-openapi.yml
- filename: mirakl-services-api-openapi.yml
  format: yaml
  label: Mirakl Services API
  slug: mirakl-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-services-api-openapi.yml
- filename: mirakl-store-api-openapi.yml
  format: yaml
  label: Mirakl Store API
  slug: mirakl-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-store-api-openapi.yml
- filename: mirakl-stores-api-openapi.yml
  format: yaml
  label: Mirakl Stores API
  slug: mirakl-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-stores-api-openapi.yml
- filename: mirakl-taxonomy-api-openapi.yml
  format: yaml
  label: Mirakl Taxonomy API
  slug: mirakl-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-taxonomy-api-openapi.yml
- filename: mirakl-users-api-openapi.yml
  format: yaml
  label: Mirakl Users API
  slug: mirakl-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-users-api-openapi.yml
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
