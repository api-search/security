---
api_key_in: []
api_specs:
- filename: oracle-retail-merchandising-openapi.yml
  format: yaml
  label: Oracle Retail Merchandising Foundation Cloud Service API
  slug: oracle-retail-merchandising-foundation-cloud-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-merchandising-openapi.yml
- filename: oracle-retail-order-management-openapi.yml
  format: yaml
  label: Oracle Retail Order Management Suite Cloud Service API
  slug: oracle-retail-order-management-suite-cloud-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/openapi/oracle-retail-order-management-openapi.yml
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
