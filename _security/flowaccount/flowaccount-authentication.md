---
api_key_in: []
api_specs:
- filename: flowaccount-batchimport-api-openapi.yml
  format: yaml
  label: FlowAccount BatchImport API
  slug: flowaccount-batchimport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-batchimport-api-openapi.yml
- filename: flowaccount-billingnote-api-openapi.yml
  format: yaml
  label: FlowAccount BillingNote API
  slug: flowaccount-billingnote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-billingnote-api-openapi.yml
- filename: flowaccount-cashinvoice-api-openapi.yml
  format: yaml
  label: FlowAccount CashInvoice API
  slug: flowaccount-cashinvoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-cashinvoice-api-openapi.yml
- filename: flowaccount-companycurrency-api-openapi.yml
  format: yaml
  label: FlowAccount CompanyCurrency API
  slug: flowaccount-companycurrency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-companycurrency-api-openapi.yml
- filename: flowaccount-contact-api-openapi.yml
  format: yaml
  label: FlowAccount Contact API
  slug: flowaccount-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-contact-api-openapi.yml
- filename: flowaccount-creditnote-api-openapi.yml
  format: yaml
  label: FlowAccount CreditNote API
  slug: flowaccount-creditnote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-creditnote-api-openapi.yml
- filename: flowaccount-debitnote-api-openapi.yml
  format: yaml
  label: FlowAccount DebitNote API
  slug: flowaccount-debitnote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-debitnote-api-openapi.yml
- filename: flowaccount-employee-api-openapi.yml
  format: yaml
  label: FlowAccount Employee API
  slug: flowaccount-employee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-employee-api-openapi.yml
- filename: flowaccount-expense-api-openapi.yml
  format: yaml
  label: FlowAccount Expense API
  slug: flowaccount-expense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-expense-api-openapi.yml
- filename: flowaccount-productcategory-api-openapi.yml
  format: yaml
  label: FlowAccount ProductCategory API
  slug: flowaccount-productcategory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-productcategory-api-openapi.yml
- filename: flowaccount-productinventory-api-openapi.yml
  format: yaml
  label: FlowAccount ProductInventory API
  slug: flowaccount-productinventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-productinventory-api-openapi.yml
- filename: flowaccount-products-api-openapi.yml
  format: yaml
  label: FlowAccount Products API
  slug: flowaccount-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-products-api-openapi.yml
- filename: flowaccount-productunit-api-openapi.yml
  format: yaml
  label: FlowAccount ProductUnit API
  slug: flowaccount-productunit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-productunit-api-openapi.yml
- filename: flowaccount-purchase-api-openapi.yml
  format: yaml
  label: FlowAccount Purchase API
  slug: flowaccount-purchase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-purchase-api-openapi.yml
- filename: flowaccount-purchaseorder-api-openapi.yml
  format: yaml
  label: FlowAccount PurchaseOrder API
  slug: flowaccount-purchaseorder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-purchaseorder-api-openapi.yml
- filename: flowaccount-quotation-api-openapi.yml
  format: yaml
  label: FlowAccount Quotation API
  slug: flowaccount-quotation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-quotation-api-openapi.yml
- filename: flowaccount-receipt-api-openapi.yml
  format: yaml
  label: FlowAccount Receipt API
  slug: flowaccount-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-receipt-api-openapi.yml
- filename: flowaccount-receivableinvoice-api-openapi.yml
  format: yaml
  label: FlowAccount ReceivableInvoice API
  slug: flowaccount-receivableinvoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-receivableinvoice-api-openapi.yml
- filename: flowaccount-taxinvoice-api-openapi.yml
  format: yaml
  label: FlowAccount TaxInvoice API
  slug: flowaccount-taxinvoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-taxinvoice-api-openapi.yml
auth_types:
- oauth2
- http
description: 'FlowAccount Open API uses OAuth 2.0 client credentials. A registered integration exchanges its client_id + client_secret at the token endpoint ({base}/token) with grant_type=client_credentials and scope=flowaccount-api to obtain a bearer access token, then sends it as `Authorization: Bearer <token>` on every request. Sandbox and Production credentials are issued separately on registration. Evidence: flowaccount/open-api apps/api/flowaccount-webhook (AuthenticationService.ts, env.json) documents grant_type=client_credentials, scope=flowaccount-api, and a tokenPost flow; the OpenAPI declares the resulting bearer scheme.'
kind: authentication
layout: security
method: searched
name: Flowaccount Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: FlowAccount secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: FlowAccount
provider_slug: flowaccount
scheme_count: 2
schemes:
- flow: clientCredentials
  name: oauth2ClientCredentials
  scopes:
  - flowaccount-api
  sources:
  - https://github.com/flowaccount/open-api
  token_endpoint: '{base}/token'
  token_endpoint_note: Base is the environment server, e.g. https://openapi.flowaccount.com/sandbox for sandbox. grant_type=client_credentials, scope=flowaccount-api, content-type application/x-www-form-urlencoded.
  type: oauth2
- bearerFormat: Reference
  description: Bearer access token obtained from the client-credentials token endpoint.
  name: bearer
  scheme: bearer
  sources:
  - openapi/flowaccount-openapi-original.json
  type: http
slug: flowaccount-authentication
source_filename: flowaccount-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/flowaccount-openapi-original.json\ndocs: https://developers.flowaccount.com/\ndescription: >-\n  FlowAccount Open API uses OAuth 2.0 client credentials. A registered integration\n  exchanges its client_id + client_secret at the token endpoint ({base}/token) with\n  grant_type=client_credentials and scope=flowaccount-api to obtain a bearer access\n  token, then sends it as `Authorization: Bearer <token>` on every request. Sandbox\n  and Production credentials are issued separately on registration. Evidence:\n  flowaccount/open-api apps/api/flowaccount-webhook (AuthenticationService.ts, env.json)\n  documents grant_type=client_credentials, scope=flowaccount-api, and a tokenPost flow;\n  the OpenAPI declares the resulting bearer scheme.\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  scopes:\n  - flowaccount-api\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n\
  \  token_endpoint: \"{base}/token\"\n  token_endpoint_note: >-\n    Base is the environment server, e.g. https://openapi.flowaccount.com/sandbox\n    for sandbox. grant_type=client_credentials, scope=flowaccount-api,\n    content-type application/x-www-form-urlencoded.\n  scopes:\n  - flowaccount-api\n  sources:\n  - https://github.com/flowaccount/open-api\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: Reference\n  description: Bearer access token obtained from the client-credentials token endpoint.\n  sources:\n  - openapi/flowaccount-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/authentication/flowaccount-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Accounting
- Invoicing
- Payroll
- Point of Sale
- SME
- Finance
- Tax
- Thailand
- Bookkeeping
---
