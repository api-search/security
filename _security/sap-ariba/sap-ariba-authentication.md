---
api_key_in: []
api_specs:
- filename: sap-ariba-invoices-api-openapi.yml
  format: yaml
  label: SAP Ariba Invoices API
  slug: sap-ariba-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/openapi/sap-ariba-invoices-api-openapi.yml
- filename: sap-ariba-purchase-order-line-items-api-openapi.yml
  format: yaml
  label: SAP Ariba Purchase Order Line Items API
  slug: sap-ariba-purchase-order-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/openapi/sap-ariba-purchase-order-line-items-api-openapi.yml
- filename: sap-ariba-purchase-orders-api-openapi.yml
  format: yaml
  label: SAP Ariba Purchase Orders API
  slug: sap-ariba-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/openapi/sap-ariba-purchase-orders-api-openapi.yml
- filename: sap-ariba-receipts-api-openapi.yml
  format: yaml
  label: SAP Ariba Receipts API
  slug: sap-ariba-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/openapi/sap-ariba-receipts-api-openapi.yml
- filename: sap-ariba-requisitions-api-openapi.yml
  format: yaml
  label: SAP Ariba Requisitions API
  slug: sap-ariba-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/openapi/sap-ariba-requisitions-api-openapi.yml
- filename: sap-ariba-suppliers-api-openapi.yml
  format: yaml
  label: SAP Ariba Suppliers API
  slug: sap-ariba-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/openapi/sap-ariba-suppliers-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Ariba Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SAP Ariba secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SAP Ariba
provider_slug: sap-ariba
scheme_count: 1
schemes:
- description: OAuth 2.0 Client Credentials flow for SAP Ariba API authentication. Obtain client credentials from the SAP Ariba Developer Portal.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.ariba.com/v2/oauth/token
  name: oauth2
  sources:
  - openapi/sap-ariba-procurement-api.yml
  type: oauth2
slug: sap-ariba-authentication
source_filename: sap-ariba-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-ariba-procurement-api.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ariba.com/v2/oauth/token\n    scopes: 0\n  description: OAuth 2.0 Client Credentials flow for SAP Ariba API authentication. Obtain client\n    credentials from the SAP Ariba Developer Portal.\n  sources:\n  - openapi/sap-ariba-procurement-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/authentication/sap-ariba-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
---
