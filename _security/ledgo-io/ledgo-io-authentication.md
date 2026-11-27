---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ledgo-io-companies-api-openapi.yml
  format: yaml
  label: Ledgo CRM Companies API
  slug: ledgo-io-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgo-io/openapi/ledgo-io-companies-api-openapi.yml
- filename: ledgo-io-contacts-api-openapi.yml
  format: yaml
  label: Ledgo CRM Contacts API
  slug: ledgo-io-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgo-io/openapi/ledgo-io-contacts-api-openapi.yml
- filename: ledgo-io-conversations-api-openapi.yml
  format: yaml
  label: Ledgo CRM Conversations API
  slug: ledgo-io-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgo-io/openapi/ledgo-io-conversations-api-openapi.yml
- filename: ledgo-io-deals-api-openapi.yml
  format: yaml
  label: Ledgo CRM Deals API
  slug: ledgo-io-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgo-io/openapi/ledgo-io-deals-api-openapi.yml
- filename: ledgo-io-leads-api-openapi.yml
  format: yaml
  label: Ledgo CRM Leads API
  slug: ledgo-io-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgo-io/openapi/ledgo-io-leads-api-openapi.yml
- filename: ledgo-io-quotes-and-invoices-api-openapi.yml
  format: yaml
  label: Ledgo CRM Quotes and invoices API
  slug: ledgo-io-quotes-and-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgo-io/openapi/ledgo-io-quotes-and-invoices-api-openapi.yml
- filename: ledgo-io-tasks-api-openapi.yml
  format: yaml
  label: Ledgo CRM Tasks API
  slug: ledgo-io-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgo-io/openapi/ledgo-io-tasks-api-openapi.yml
- filename: ledgo-io-workspace-api-openapi.yml
  format: yaml
  label: Ledgo CRM Workspace API
  slug: ledgo-io-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgo-io/openapi/ledgo-io-workspace-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ledgo CRM Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ledgo CRM secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ledgo CRM
provider_slug: ledgo-io
scheme_count: 1
schemes:
- description: An API key (agk_…) created in Settings → Integrations → REST API.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/ledgo-io-openapi.json
  type: http
slug: ledgo-io-authentication
source_filename: ledgo-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/ledgo-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: An API key (agk_…) created in Settings → Integrations → REST API.\n  sources:\n  - openapi/ledgo-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/ledgo-io/authentication/ledgo-io-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Artificial Intelligence
- Messaging
- Sales
- Automation
- Software-as-a-Service
---
