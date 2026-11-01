---
anonymous_access: false
api_key_in: []
api_specs:
- filename: storecove-additionaltaxidentifiers-api-openapi.yml
  format: yaml
  label: Storecove Additional Tax Identifiers API
  slug: storecove-additionaltaxidentifiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-additionaltaxidentifiers-api-openapi.yml
- filename: storecove-administrations-api-openapi.yml
  format: yaml
  label: Storecove Administrations API
  slug: storecove-administrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-administrations-api-openapi.yml
- filename: storecove-c5activation-api-openapi.yml
  format: yaml
  label: Storecove C5Activation API
  slug: storecove-c5activation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-c5activation-api-openapi.yml
- filename: storecove-discovery-api-openapi.yml
  format: yaml
  label: Storecove Discovery API
  slug: storecove-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-discovery-api-openapi.yml
- filename: storecove-invoicesubmissions-api-openapi.yml
  format: yaml
  label: Storecove Invoice Submissions API
  slug: storecove-invoicesubmissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-invoicesubmissions-api-openapi.yml
- filename: storecove-legalentities-api-openapi.yml
  format: yaml
  label: Storecove Legal Entities API
  slug: storecove-legalentities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-legalentities-api-openapi.yml
- filename: storecove-peppolidentifiers-api-openapi.yml
  format: yaml
  label: Storecove Peppol Identifiers API
  slug: storecove-peppolidentifiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-peppolidentifiers-api-openapi.yml
- filename: storecove-purchaseinvoices-api-openapi.yml
  format: yaml
  label: Storecove Purchase Invoices API
  slug: storecove-purchaseinvoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-purchaseinvoices-api-openapi.yml
- filename: storecove-receiveddocuments-api-openapi.yml
  format: yaml
  label: Storecove Received Documents API
  slug: storecove-receiveddocuments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-receiveddocuments-api-openapi.yml
- filename: storecove-webhookinstances-api-openapi.yml
  format: yaml
  label: Storecove Webhook Instances API
  slug: storecove-webhookinstances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-webhookinstances-api-openapi.yml
- filename: storecove-document-submissions-api-openapi.yml
  format: yaml
  label: Storecove document submissions API
  slug: storecove-document-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-document-submissions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Storecove Authentication
name_suffix: Authentication
oauth_flows: []
overview: Storecove secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Storecove
provider_slug: storecove
scheme_count: 1
schemes:
- bearerFormat: Bearer 9999999999999999999999999999999999999999999999999999999999999999
  description: See https://datatracker.ietf.org/doc/html/rfc6750#section-2.1 for details
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/storecove-openapi.yml
  type: http
slug: storecove-authentication
source_filename: storecove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/storecove-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Bearer 9999999999999999999999999999999999999999999999999999999999999999\n  description: See https://datatracker.ietf.org/doc/html/rfc6750#section-2.1 for details\n  sources:\n  - openapi/storecove-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/storecove/authentication/storecove-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- E-Invoicing
- PEPPOL
- Tax Compliance
- Invoicing
- Accounting
- ERP Integration
- Fintech
---
