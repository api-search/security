---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jupiterinvoice-com-customers-api-openapi.yml
  format: yaml
  label: JupiterInvoice Customers API
  slug: jupiterinvoice-com-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiterinvoice-com/openapi/jupiterinvoice-com-customers-api-openapi.yml
- filename: jupiterinvoice-com-invoices-api-openapi.yml
  format: yaml
  label: JupiterInvoice Invoices API
  slug: jupiterinvoice-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiterinvoice-com/openapi/jupiterinvoice-com-invoices-api-openapi.yml
- filename: jupiterinvoice-com-webhooks-api-openapi.yml
  format: yaml
  label: JupiterInvoice Webhooks API
  slug: jupiterinvoice-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiterinvoice-com/openapi/jupiterinvoice-com-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: JupiterInvoice Authentication
name_suffix: Authentication
oauth_flows: []
overview: JupiterInvoice secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JupiterInvoice
provider_slug: jupiterinvoice-com
scheme_count: 1
schemes:
- bearerFormat: API key (jk_live_*)
  description: Mint a key on the Integrations page (https://jupiterinvoice.com/integrations#api-keys). Shown once.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/jupiterinvoice-com-openapi.yml
  type: http
slug: jupiterinvoice-com-authentication
source_filename: jupiterinvoice-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/jupiterinvoice-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key (jk_live_*)\n  description: Mint a key on the Integrations page (https://jupiterinvoice.com/integrations#api-keys).\n    Shown once.\n  sources:\n  - openapi/jupiterinvoice-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/jupiterinvoice-com/authentication/jupiterinvoice-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Invoicing
- Fintech
- Software-as-a-Service
- Free
---
