---
api_key_in: []
api_specs:
- filename: microsoft-dynamics-accounts-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Accounts API
  slug: microsoft-dynamics-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-accounts-api-openapi.yml
- filename: microsoft-dynamics-activities-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Activities API
  slug: microsoft-dynamics-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-activities-api-openapi.yml
- filename: microsoft-dynamics-cases-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Cases API
  slug: microsoft-dynamics-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-cases-api-openapi.yml
- filename: microsoft-dynamics-companies-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Companies API
  slug: microsoft-dynamics-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-companies-api-openapi.yml
- filename: microsoft-dynamics-contacts-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Contacts API
  slug: microsoft-dynamics-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-contacts-api-openapi.yml
- filename: microsoft-dynamics-customers-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Customers API
  slug: microsoft-dynamics-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-customers-api-openapi.yml
- filename: microsoft-dynamics-employees-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Employees API
  slug: microsoft-dynamics-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-employees-api-openapi.yml
- filename: microsoft-dynamics-general-ledger-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics General Ledger API
  slug: microsoft-dynamics-general-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-general-ledger-api-openapi.yml
- filename: microsoft-dynamics-human-resources-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Human Resources API
  slug: microsoft-dynamics-human-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-human-resources-api-openapi.yml
- filename: microsoft-dynamics-items-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Items API
  slug: microsoft-dynamics-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-items-api-openapi.yml
- filename: microsoft-dynamics-journals-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Journals API
  slug: microsoft-dynamics-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-journals-api-openapi.yml
- filename: microsoft-dynamics-leads-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Leads API
  slug: microsoft-dynamics-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-leads-api-openapi.yml
- filename: microsoft-dynamics-opportunities-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Opportunities API
  slug: microsoft-dynamics-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-opportunities-api-openapi.yml
- filename: microsoft-dynamics-products-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Products API
  slug: microsoft-dynamics-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-products-api-openapi.yml
- filename: microsoft-dynamics-purchase-invoices-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Purchase Invoices API
  slug: microsoft-dynamics-purchase-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-purchase-invoices-api-openapi.yml
- filename: microsoft-dynamics-purchase-orders-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Purchase Orders API
  slug: microsoft-dynamics-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-purchase-orders-api-openapi.yml
- filename: microsoft-dynamics-sales-invoices-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Sales Invoices API
  slug: microsoft-dynamics-sales-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-sales-invoices-api-openapi.yml
- filename: microsoft-dynamics-sales-orders-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Sales Orders API
  slug: microsoft-dynamics-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-sales-orders-api-openapi.yml
- filename: microsoft-dynamics-vendors-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics Vendors API
  slug: microsoft-dynamics-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-vendors-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Dynamics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Dynamics secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
scheme_count: 2
schemes:
- description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-dynamics-business-central-openapi.yml
  - openapi/microsoft-dynamics-dataverse-openapi.yml
  type: oauth2
- description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-dynamics-finance-operations-openapi.yml
  type: oauth2
slug: microsoft-dynamics-authentication
source_filename: microsoft-dynamics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-dynamics-business-central-openapi.yml, openapi/microsoft-dynamics-dataverse-openapi.yml,\n  openapi/microsoft-dynamics-finance-operations-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.\n  sources:\n  - openapi/microsoft-dynamics-business-central-openapi.yml\n  - openapi/microsoft-dynamics-dataverse-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID (Azure AD) OAuth 2.0\
  \ authentication.\n  sources:\n  - openapi/microsoft-dynamics-finance-operations-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/authentication/microsoft-dynamics-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- CRM
- ERP
- Microsoft Dynamics
---
