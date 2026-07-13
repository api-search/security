---
api_key_in: []
api_specs:
- filename: overview
  format: yaml
  label: Commerce Web Services API
  slug: commerce-web-services-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/commerce_web_services/overview
- filename: sap-commerce-cloud-assisted-service-openapi.yml
  format: yaml
  label: Assisted Service Module API
  slug: assisted-service-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/openapi/sap-commerce-cloud-assisted-service-openapi.yml
- filename: sap-commerce-cloud-integration-openapi.yml
  format: yaml
  label: Integration API
  slug: integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/openapi/sap-commerce-cloud-integration-openapi.yml
- filename: sap-commerce-cloud-admin-openapi.yml
  format: yaml
  label: Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/openapi/sap-commerce-cloud-admin-openapi.yml
- filename: sap-commerce-cloud-product-content-management-openapi.yml
  format: yaml
  label: Product Content Management API
  slug: product-content-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/openapi/sap-commerce-cloud-product-content-management-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Commerce Cloud Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: SAP Commerce Cloud secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: SAP Commerce Cloud
provider_slug: sap-commerce-cloud
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication for SAP Commerce Cloud Admin API
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token
  name: oauth2
  sources:
  - openapi/sap-commerce-cloud-admin-openapi.yml
  - openapi/sap-commerce-cloud-assisted-service-openapi.yml
  - openapi/sap-commerce-cloud-integration-openapi.yml
  - openapi/sap-commerce-cloud-product-content-management-openapi.yml
  type: oauth2
- description: OAuth 2.0 authentication for SAP Commerce Cloud
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token
  - flow: password
    scopes: 1
    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token
  name: oauth2
  sources:
  - openapi/sap-commerce-cloud-commerce-web-services-openapi.yml
  type: oauth2
slug: sap-commerce-cloud-authentication
source_filename: sap-commerce-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-commerce-cloud-admin-openapi.yml, openapi/sap-commerce-cloud-assisted-service-openapi.yml,\n  openapi/sap-commerce-cloud-commerce-web-services-openapi.yml, openapi/sap-commerce-cloud-integration-openapi.yml,\n  openapi/sap-commerce-cloud-product-content-management-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - password\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token\n    scopes: 1\n  description: OAuth 2.0 authentication for SAP Commerce Cloud Admin API\n  sources:\n  - openapi/sap-commerce-cloud-admin-openapi.yml\n  - openapi/sap-commerce-cloud-assisted-service-openapi.yml\n  - openapi/sap-commerce-cloud-integration-openapi.yml\n  - openapi/sap-commerce-cloud-product-content-management-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow:\
  \ clientCredentials\n    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token\n    scopes: 1\n  - flow: password\n    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token\n    scopes: 1\n  description: OAuth 2.0 authentication for SAP Commerce Cloud\n  sources:\n  - openapi/sap-commerce-cloud-commerce-web-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/authentication/sap-commerce-cloud-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- B2B
- B2C
- Commerce
- Customer Experience
- Ecommerce
- Omnichannel
- Retail
---
