---
api_key_in: []
api_specs:
- filename: overview
  format: yaml
  label: SAP S/4HANA Business Partner API
  slug: sap-s4hana-business-partner-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_BUSINESS_PARTNER/overview
- filename: sap-s4hana-sales-order-openapi.yml
  format: yaml
  label: SAP S/4HANA Sales Order API
  slug: sap-s4hana-sales-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-sales-order-openapi.yml
- filename: overview
  format: yaml
  label: SAP S/4HANA Purchase Order API
  slug: sap-s4hana-purchase-order-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_PURCHASEORDER_PROCESS_SRV/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Material Document API
  slug: sap-s4hana-material-document-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_MATERIAL_DOCUMENT_SRV/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Product Master API
  slug: sap-s4hana-product-master-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_PRODUCT_SRV/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Journal Entry API
  slug: sap-s4hana-journal-entry-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_JOURNALENTRY_SRV/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Billing Document API
  slug: sap-s4hana-billing-document-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_BILLING_DOCUMENT_SRV/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Supplier Invoice API
  slug: sap-s4hana-supplier-invoice-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_SUPPLIERINVOICE_PROCESS_SRV/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Customer Return API
  slug: sap-s4hana-customer-return-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_CUSTOMER_RETURN_SRV/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Purchase Requisition API
  slug: sap-s4hana-purchase-requisition-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_PURCHASEREQ_PROCESS_SRV/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Outbound Delivery API
  slug: sap-s4hana-outbound-delivery-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_OUTBOUND_DELIVERY_SRV_0002/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Inbound Delivery API
  slug: sap-s4hana-inbound-delivery-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_INBOUND_DELIVERY_SRV_0002/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Cost Center API
  slug: sap-s4hana-cost-center-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_COSTCENTER_SRV/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA GL Account API
  slug: sap-s4hana-gl-account-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_GLACCOUNTINCHARTOFACCOUNTS_SRV/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Bank Master API
  slug: sap-s4hana-bank-master-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_BANKDETAIL_SRV/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Production Order API
  slug: sap-s4hana-production-order-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_PRODUCTION_ORDER_2_SRV/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Maintenance Order API
  slug: sap-s4hana-maintenance-order-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_MAINTENANCEORDER/overview
- filename: overview
  format: yaml
  label: SAP S/4HANA Workforce Timesheet API
  slug: sap-s4hana-workforce-timesheet-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_MANAGE_WORKFORCE_TIMESHEET/overview
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap S4Hana Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SAP S/4HANA secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
scheme_count: 2
schemes:
- description: Basic authentication using SAP user credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/sap-s4hana-sales-order-openapi.yml
  type: http
- description: OAuth 2.0 authentication for SAP S/4HANA Cloud
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  sources:
  - openapi/sap-s4hana-sales-order-openapi.yml
  type: oauth2
slug: sap-s4hana-authentication
source_filename: sap-s4hana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-s4hana-sales-order-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication using SAP user credentials\n  sources:\n  - openapi/sap-s4hana-sales-order-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token\n    scopes: 1\n  description: OAuth 2.0 authentication for SAP S/4HANA Cloud\n  sources:\n  - openapi/sap-s4hana-sales-order-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/authentication/sap-s4hana-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Business Applications
- Cloud
- Enterprise Resource Planning
- ERP
- Finance
- Human Resources
- Inventory
- Logistics
- Manufacturing
- Plant Maintenance
- Procurement
- S/4HANA
- Sales
- SAP
---
