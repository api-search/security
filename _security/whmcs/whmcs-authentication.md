---
api_key_in:
- query
api_specs:
- filename: whmcs-openapi.yml
  format: yaml
  label: WHMCS API
  slug: whmcs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whmcs/main/openapi/whmcs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Whmcs Authentication
name_suffix: Authentication
oauth_flows: []
overview: WHMCS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WHMCS
provider_slug: whmcs
scheme_count: 1
schemes:
- description: WHMCS API credentials. Provide identifier and secret parameters in the POST request body, along with the action parameter.
  in: query
  name: ApiCredentials
  parameter: identifier
  sources:
  - openapi/whmcs-openapi.yml
  type: apiKey
slug: whmcs-authentication
source_filename: whmcs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/whmcs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiCredentials\n  type: apiKey\n  in: query\n  parameter: identifier\n  description: WHMCS API credentials. Provide identifier and secret parameters in the POST request\n    body, along with the action parameter.\n  sources:\n  - openapi/whmcs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whmcs/refs/heads/main/authentication/whmcs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web Hosting
- Billing Automation
- Client Management
- Domain Management
- Support Tickets
- Provisioning
---
