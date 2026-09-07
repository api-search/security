---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eci-solutions-erp-v2-1-openapi.json
  format: json
  label: ECI Manufacturing ERP API
  slug: eci-solutions-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-erp-v2-1-openapi.json
- filename: eci-solutions-jobboss2-openapi.json
  format: json
  label: JobBOSS² Public API
  slug: eci-solutions-jobboss2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-jobboss2-openapi.json
- filename: eci-solutions-m1-openapi.json
  format: json
  label: M1 Public API
  slug: eci-solutions-m1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-m1-openapi.json
- filename: eci-solutions-management-openapi.json
  format: json
  label: ECI MFG Integration Management API
  slug: eci-solutions-integration-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-management-openapi.json
- filename: eci-solutions-authentication-openapi.json
  format: json
  label: ECI Authentication API
  slug: eci-solutions-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-authentication-openapi.json
- filename: eci-solutions-payment-openapi.json
  format: json
  label: ECI MFG Payment API
  slug: eci-solutions-payment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-payment-openapi.json
- filename: eci-solutions-financial-v2-openapi.json
  format: json
  label: ECI Financial Integration API
  slug: eci-solutions-financial
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-financial-v2-openapi.json
- filename: eci-solutions-ecommerce-openapi.json
  format: json
  label: ECI EvolutionX Ecommerce API
  slug: eci-solutions-ecommerce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-ecommerce-openapi.json
- filename: eci-solutions-einvoice-openapi.json
  format: json
  label: ECI Einvoice API
  slug: eci-solutions-einvoice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-einvoice-openapi.json
- filename: eci-solutions-shipping-openapi.json
  format: json
  label: ECI Shipping API
  slug: eci-solutions-shipping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-shipping-openapi.json
- filename: eci-solutions-currency-openapi.json
  format: json
  label: ECI Currency Data API
  slug: eci-solutions-currency
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-currency-openapi.json
- filename: eci-solutions-apar-commerce-openapi.json
  format: json
  label: ECI AP/AR Commerce Automation API
  slug: eci-solutions-apar-commerce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-apar-commerce-openapi.json
- filename: eci-solutions-office-openapi.json
  format: json
  label: ECI Office Integration API
  slug: eci-solutions-office
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-office-openapi.json
- filename: eci-solutions-notification-openapi.json
  format: json
  label: ECI Notification API
  slug: eci-solutions-notification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-notification-openapi.json
- filename: eci-solutions-lasso-crm-openapi.yml
  format: yaml
  label: Lasso CRM API
  slug: eci-solutions-lasso-crm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-lasso-crm-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: derived
name: Eci Solutions Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: ECI Solutions secures its APIs with http, oauth2, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: ECI Solutions
provider_slug: eci-solutions
scheme_count: 5
schemes:
- description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine Management Console
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  sources:
  - openapi/eci-solutions-apar-commerce-openapi.json
  - openapi/eci-solutions-currency-openapi.json
  - openapi/eci-solutions-ecommerce-openapi.json
  - openapi/eci-solutions-einvoice-openapi.json
  - openapi/eci-solutions-erp-v1-openapi.json
  - openapi/eci-solutions-erp-v2-1-openapi.json
  - openapi/eci-solutions-erp-v2-openapi.json
  - openapi/eci-solutions-financial-v1-openapi.json
  - openapi/eci-solutions-financial-v2-openapi.json
  - openapi/eci-solutions-jobboss2-openapi.json
  - openapi/eci-solutions-m1-openapi.json
  - openapi/eci-solutions-notification-openapi.json
  - openapi/eci-solutions-office-openapi.json
  - openapi/eci-solutions-payment-openapi.json
  - openapi/eci-solutions-shipping-openapi.json
  type: oauth2
- description: Use id_token obtained from OpenID Connect flow.
  name: oidc
  openIdConnectUrl: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_9IYBf4TpD/.well-known/openid-configuration
  sources:
  - openapi/eci-solutions-authentication-openapi.json
  - openapi/eci-solutions-management-openapi.json
  type: openIdConnect
- description: Username is ClientID, Password is Client Secret.
  name: Basic
  scheme: Basic
  sources:
  - openapi/eci-solutions-authentication-openapi.json
  - openapi/eci-solutions-management-openapi.json
  type: http
- bearerFormat: JWT
  name: JwtAuthorizer
  scheme: bearer
  sources:
  - openapi/eci-solutions-lasso-crm-openapi.yml
  type: http
- bearerFormat: JWT
  description: Enter your token
  name: Auth0
  scheme: Bearer
  sources:
  - openapi/eci-solutions-notification-openapi.json
  type: http
slug: eci-solutions-authentication
source_filename: eci-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: openapi/eci-solutions-apar-commerce-openapi.json, openapi/eci-solutions-authentication-openapi.json,\n  openapi/eci-solutions-currency-openapi.json, openapi/eci-solutions-ecommerce-openapi.json,\n  openapi/eci-solutions-einvoice-openapi.json, openapi/eci-solutions-erp-v1-openapi.json, openapi/eci-solutions-erp-v2-1-openapi.json,\n  openapi/eci-solutions-erp-v2-openapi.json, openapi/eci-solutions-financial-v1-openapi.json,\n  openapi/eci-solutions-financial-v2-openapi.json, openapi/eci-solutions-jobboss2-openapi.json,\n  openapi/eci-solutions-lasso-crm-openapi.yml ...\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Bearer\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n    scopes: 1\n  description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration\
  \ Engine\n    Management Console\n  sources:\n  - openapi/eci-solutions-apar-commerce-openapi.json\n  - openapi/eci-solutions-currency-openapi.json\n  - openapi/eci-solutions-ecommerce-openapi.json\n  - openapi/eci-solutions-einvoice-openapi.json\n  - openapi/eci-solutions-erp-v1-openapi.json\n  - openapi/eci-solutions-erp-v2-1-openapi.json\n  - openapi/eci-solutions-erp-v2-openapi.json\n  - openapi/eci-solutions-financial-v1-openapi.json\n  - openapi/eci-solutions-financial-v2-openapi.json\n  - openapi/eci-solutions-jobboss2-openapi.json\n  - openapi/eci-solutions-m1-openapi.json\n  - openapi/eci-solutions-notification-openapi.json\n  - openapi/eci-solutions-office-openapi.json\n  - openapi/eci-solutions-payment-openapi.json\n  - openapi/eci-solutions-shipping-openapi.json\n- name: oidc\n  type: openIdConnect\n  openIdConnectUrl: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_9IYBf4TpD/.well-known/openid-configuration\n  description: Use id_token obtained from OpenID Connect flow.\n\
  \  sources:\n  - openapi/eci-solutions-authentication-openapi.json\n  - openapi/eci-solutions-management-openapi.json\n- name: Basic\n  type: http\n  scheme: Basic\n  description: Username is ClientID, Password is Client Secret.\n  sources:\n  - openapi/eci-solutions-authentication-openapi.json\n  - openapi/eci-solutions-management-openapi.json\n- name: JwtAuthorizer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/eci-solutions-lasso-crm-openapi.yml\n- name: Auth0\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description: Enter your token\n  sources:\n  - openapi/eci-solutions-notification-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/authentication/eci-solutions-authentication.yml
summary_line: http/oauth2/openIdConnect · 5 schemes
tags:
- Accounting
- Building Supply
- Business Management
- CRM
- Construction
- Distribution
- E-Commerce
- ERP
- Field Service
- Inventory
- Manufacturing
- Payments
- Retail
- Shipping
---
