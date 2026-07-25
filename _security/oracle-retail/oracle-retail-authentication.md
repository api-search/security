---
api_key_in: []
api_specs:
- filename: oracle-retail-fulfillment-api-openapi.yml
  format: yaml
  label: Oracle Retail Fulfillment API
  slug: oracle-retail-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-fulfillment-api-openapi.yml
- filename: oracle-retail-inventory-api-openapi.yml
  format: yaml
  label: Oracle Retail Inventory API
  slug: oracle-retail-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-inventory-api-openapi.yml
- filename: oracle-retail-items-api-openapi.yml
  format: yaml
  label: Oracle Retail Items API
  slug: oracle-retail-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-items-api-openapi.yml
- filename: oracle-retail-orders-api-openapi.yml
  format: yaml
  label: Oracle Retail Orders API
  slug: oracle-retail-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-orders-api-openapi.yml
- filename: oracle-retail-purchaseorders-api-openapi.yml
  format: yaml
  label: Oracle Retail PurchaseOrders API
  slug: oracle-retail-purchaseorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-purchaseorders-api-openapi.yml
- filename: oracle-retail-returns-api-openapi.yml
  format: yaml
  label: Oracle Retail Returns API
  slug: oracle-retail-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-returns-api-openapi.yml
- filename: oracle-retail-suppliers-api-openapi.yml
  format: yaml
  label: Oracle Retail Suppliers API
  slug: oracle-retail-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-suppliers-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Retail Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Oracle Retail secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Oracle Retail
provider_slug: oracle-retail
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://identity.oraclecloud.com/oauth2/v1/token
  name: oauth2
  sources:
  - openapi/oracle-retail-merchandising-openapi.yml
  - openapi/oracle-retail-order-management-openapi.yml
  type: oauth2
slug: oracle-retail-authentication
source_filename: oracle-retail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-retail-merchandising-openapi.yml, openapi/oracle-retail-order-management-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.oraclecloud.com/oauth2/v1/token\n    scopes: 2\n  sources:\n  - openapi/oracle-retail-merchandising-openapi.yml\n  - openapi/oracle-retail-order-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/authentication/oracle-retail-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Retail
- Merchandising
- Order Management
- Pricing
- Inventory
- Point of Sale
- Omnichannel
- Oracle
---
