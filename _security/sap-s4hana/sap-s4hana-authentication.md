---
api_key_in: []
api_specs:
- filename: sap-s4hana-partners-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Partners API
  slug: sap-s4hana-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-partners-api-openapi.yml
- filename: sap-s4hana-pricing-elements-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Pricing Elements API
  slug: sap-s4hana-pricing-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-pricing-elements-api-openapi.yml
- filename: sap-s4hana-sales-order-items-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Sales Order Items API
  slug: sap-s4hana-sales-order-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-sales-order-items-api-openapi.yml
- filename: sap-s4hana-sales-orders-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Sales Orders API
  slug: sap-s4hana-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-sales-orders-api-openapi.yml
- filename: sap-s4hana-schedule-lines-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Schedule Lines API
  slug: sap-s4hana-schedule-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-schedule-lines-api-openapi.yml
- filename: sap-s4hana-text-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Text API
  slug: sap-s4hana-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-text-api-openapi.yml
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
