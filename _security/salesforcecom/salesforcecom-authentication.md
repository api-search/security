---
api_key_in: []
api_specs:
- filename: salesforcecom-rest-openapi.yml
  format: yaml
  label: Salesforce REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforcecom/refs/heads/main/openapi/salesforcecom-rest-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Salesforcecom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Salesforce secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Salesforce
provider_slug: salesforcecom
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer access token obtained via Salesforce Connected App
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salesforcecom-rest-openapi.yml
  type: http
slug: salesforcecom-authentication
source_filename: salesforcecom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforcecom-rest-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer access token obtained via Salesforce Connected App\n  sources:\n  - openapi/salesforcecom-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforcecom/refs/heads/main/authentication/salesforcecom-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Cloud
- Sales
- Marketing
- Automation
- AI
- Fortune 500
---
