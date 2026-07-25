---
api_key_in: []
api_specs:
- filename: workist-delivery-notes-api-openapi.yml
  format: yaml
  label: Workist Delivery Notes API
  slug: workist-delivery-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workist/refs/heads/main/openapi/workist-delivery-notes-api-openapi.yml
- filename: workist-invoices-api-openapi.yml
  format: yaml
  label: Workist Invoices API
  slug: workist-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workist/refs/heads/main/openapi/workist-invoices-api-openapi.yml
- filename: workist-list-of-services-api-openapi.yml
  format: yaml
  label: Workist List Of Services API
  slug: workist-list-of-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workist/refs/heads/main/openapi/workist-list-of-services-api-openapi.yml
- filename: workist-master-data-api-openapi.yml
  format: yaml
  label: Workist Master Data API
  slug: workist-master-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workist/refs/heads/main/openapi/workist-master-data-api-openapi.yml
- filename: workist-order-confirmations-api-openapi.yml
  format: yaml
  label: Workist Order Confirmations API
  slug: workist-order-confirmations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workist/refs/heads/main/openapi/workist-order-confirmations-api-openapi.yml
- filename: workist-orders-api-openapi.yml
  format: yaml
  label: Workist Orders API
  slug: workist-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workist/refs/heads/main/openapi/workist-orders-api-openapi.yml
- filename: workist-property-bills-api-openapi.yml
  format: yaml
  label: Workist Property Bills API
  slug: workist-property-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workist/refs/heads/main/openapi/workist-property-bills-api-openapi.yml
- filename: workist-rfq-api-openapi.yml
  format: yaml
  label: Workist Rfq API
  slug: workist-rfq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workist/refs/heads/main/openapi/workist-rfq-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Workist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Workist secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Workist
provider_slug: workist
scheme_count: 1
schemes:
- header: 'Authorization: Bearer <token>'
  name: BearerAuthentication
  scheme: bearer
  sources:
  - openapi/workist-integrations-openapi-original.yml
  token_source: https://wb.workist.com/customer/integrations/api-integrations
  type: http
slug: workist-authentication
source_filename: workist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/workist-integrations-openapi-original.yml\ndocs: https://docs.workist.com/en/docs/api-documentation/quickstart/\nsummary:\n  types:\n  - http\n  notes: >-\n    Bearer token authentication. Tokens are created by the customer in the\n    Workist Workbench under Integrations > API Integrations\n    (https://wb.workist.com/customer/integrations/api-integrations) and sent\n    on every request as \"Authorization: Bearer <token>\". No OAuth flows or\n    scopes are published.\nschemes:\n- name: BearerAuthentication\n  type: http\n  scheme: bearer\n  token_source: https://wb.workist.com/customer/integrations/api-integrations\n  header: 'Authorization: Bearer <token>'\n  sources:\n  - openapi/workist-integrations-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workist/refs/heads/main/authentication/workist-authentication.yml
summary_line: http · 1 scheme
tags:
- Documents
- Document Processing
- Artificial Intelligence
- Automation
- Orders
- Invoices
- ERP
- B2B
- Master Data
---
