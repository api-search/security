---
api_key_in:
- header
api_specs:
- filename: feathery-account-api-openapi.yml
  format: yaml
  label: Feathery Account API
  slug: feathery-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-account-api-openapi.yml
- filename: feathery-data-hubs-api-openapi.yml
  format: yaml
  label: Feathery Data Hubs API
  slug: feathery-data-hubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-data-hubs-api-openapi.yml
- filename: feathery-document-intelligence-api-openapi.yml
  format: yaml
  label: Feathery Document Intelligence API
  slug: feathery-document-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-document-intelligence-api-openapi.yml
- filename: feathery-document-templates-api-openapi.yml
  format: yaml
  label: Feathery Document Templates API
  slug: feathery-document-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-document-templates-api-openapi.yml
- filename: feathery-end-users-api-openapi.yml
  format: yaml
  label: Feathery End Users API
  slug: feathery-end-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-end-users-api-openapi.yml
- filename: feathery-forms-api-openapi.yml
  format: yaml
  label: Feathery Forms API
  slug: feathery-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-forms-api-openapi.yml
- filename: feathery-hidden-fields-api-openapi.yml
  format: yaml
  label: Feathery Hidden Fields API
  slug: feathery-hidden-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-hidden-fields-api-openapi.yml
- filename: feathery-logs-api-openapi.yml
  format: yaml
  label: Feathery Logs API
  slug: feathery-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-logs-api-openapi.yml
- filename: feathery-workspaces-api-openapi.yml
  format: yaml
  label: Feathery Workspaces API
  slug: feathery-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/openapi/feathery-workspaces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Feathery Authentication
name_suffix: Authentication
oauth_flows: []
overview: Feathery secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Feathery
provider_slug: feathery
scheme_count: 1
schemes:
- description: 'Token-based authentication. Format: Token <API KEY>'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/feathery-rest-api-openapi.yml
  type: apiKey
slug: feathery-authentication
source_filename: feathery-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/feathery-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token-based authentication. Format: Token <API KEY>'\n  sources:\n  - openapi/feathery-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feathery/refs/heads/main/authentication/feathery-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Forms
- Form Builder
- Multi-Step Forms
- Document Intelligence
- Artificial Intelligence
- Financial-Services
- Insurance
- Wealth Management
- E-Signature
- Workflows
- Data Intake
- Submissions
- Payments
- Authentication
---
