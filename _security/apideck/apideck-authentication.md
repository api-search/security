---
api_key_in:
- header
api_specs:
- filename: apideck-accounting-openapi.yml
  format: yaml
  label: Apideck Accounting API
  slug: accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apideck/refs/heads/main/openapi/apideck-accounting-openapi.yml
- filename: apideck-crm-openapi.yml
  format: yaml
  label: Apideck CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apideck/refs/heads/main/openapi/apideck-crm-openapi.yml
- filename: apideck-hris-openapi.yml
  format: yaml
  label: Apideck HRIS API
  slug: hris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apideck/refs/heads/main/openapi/apideck-hris-openapi.yml
- filename: ats.yml
  format: yaml
  label: Apideck ATS API
  slug: ats-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/ats.yml
- filename: apideck-file-storage-openapi.yml
  format: yaml
  label: Apideck File Storage API
  slug: file-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apideck/refs/heads/main/openapi/apideck-file-storage-openapi.yml
- filename: ecommerce.yml
  format: yaml
  label: Apideck Ecommerce API
  slug: ecommerce-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/ecommerce.yml
- filename: pos.yml
  format: yaml
  label: Apideck POS API
  slug: pos-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/pos.yml
- filename: issue-tracking.yml
  format: yaml
  label: Apideck Issue Tracking API
  slug: issue-tracking-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/issue-tracking.yml
- filename: lead.yml
  format: yaml
  label: Apideck Lead API
  slug: lead-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/lead.yml
- filename: sms.yml
  format: yaml
  label: Apideck SMS API
  slug: sms-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/sms.yml
- filename: vault.yml
  format: yaml
  label: Apideck Vault API
  slug: vault-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/vault.yml
- filename: webhook.yml
  format: yaml
  label: Apideck Webhook API
  slug: webhook-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/webhook.yml
- filename: connector.yml
  format: yaml
  label: Apideck Connector API
  slug: connector-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/connector.yml
- filename: proxy.yml
  format: yaml
  label: Apideck Proxy API
  slug: proxy-api
  spec_type: OpenAPI
  url: https://specs.apideck.com/proxy.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apideck Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apideck secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Apideck
provider_slug: apideck
scheme_count: 3
schemes:
- description: 'To access our API, you need to sign up and obtain your unique API key. Each Unify application is assigned a single API key. You can locate your API key in the Configuration Settings section of your Apideck application. Additionally, your application’s application_id is available on the same page.


    Authenticate your API requests by including your test or live secret API key in the request header.


    '
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/apideck-accounting-openapi.yml
  - openapi/apideck-crm-openapi.yml
  - openapi/apideck-file-storage-openapi.yml
  - openapi/apideck-hris-openapi.yml
  type: apiKey
- description: The ID of your Unify application
  in: header
  name: applicationId
  parameter: x-apideck-app-id
  sources:
  - openapi/apideck-crm-openapi.yml
  type: apiKey
- description: The ID of the consumer which you want to get or push data from
  in: header
  name: consumerId
  parameter: x-apideck-consumer-id
  sources:
  - openapi/apideck-crm-openapi.yml
  type: apiKey
slug: apideck-authentication
source_filename: apideck-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apideck-accounting-openapi.yml, openapi/apideck-crm-openapi.yml, openapi/apideck-file-storage-openapi.yml,\n  openapi/apideck-hris-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |+\n    To access our API, you need to sign up and obtain your unique API key. Each Unify application is assigned a single API key. You can locate your API key in the Configuration Settings section of your Apideck application. Additionally, your application’s application_id is available on the same page.\n\n    Authenticate your API requests by including your test or live secret API key in the request header.\n\n  sources:\n  - openapi/apideck-accounting-openapi.yml\n  - openapi/apideck-crm-openapi.yml\n  - openapi/apideck-file-storage-openapi.yml\n  - openapi/apideck-hris-openapi.yml\n- name: applicationId\n  type: apiKey\n\
  \  in: header\n  parameter: x-apideck-app-id\n  description: The ID of your Unify application\n  sources:\n  - openapi/apideck-crm-openapi.yml\n- name: consumerId\n  type: apiKey\n  in: header\n  parameter: x-apideck-consumer-id\n  description: The ID of the consumer which you want to get or push data from\n  sources:\n  - openapi/apideck-crm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apideck/refs/heads/main/authentication/apideck-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Integrations
- Unified API
---
