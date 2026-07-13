---
api_key_in:
- header
api_specs:
- filename: frappe_api-docs
  format: yaml
  label: ERPNext REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://github.com/alyf-de/frappe_api-docs
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Erpnext Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ERPNext secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ERPNext
provider_slug: erpnext
scheme_count: 3
schemes:
- description: 'Get your API keys at User -> Api Access -> Generate Keys.

    "headers = {''Authorization'': ''token <api_key>:<api_secret>''}"'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/openapi.yaml
  type: apiKey
- description: 'Get your API keys at User -> Api Access -> Generate Keys.

    username = api_key; password = api_secret

    [More info](https://frappe.io/docs/user/en/guides/integration/token_based_auth)'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/openapi.yaml
  type: http
- description: "This API uses OAuth 2 with the authorization code flow. \n[More info]https://frappe.io/docs/user/en/guides/integration/using_oauth)"
  flows:
  - authorizationUrl: /method/frappe.integrations.oauth2.authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: /method/frappe.integrations.oauth2.get_token
  name: oAuth2
  sources:
  - openapi/openapi.yaml
  type: oauth2
slug: erpnext-authentication
source_filename: erpnext-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Get your API keys at User -> Api Access -> Generate Keys.\n    \"headers = {'Authorization': 'token <api_key>:<api_secret>'}\"\n  sources:\n  - openapi/openapi.yaml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Get your API keys at User -> Api Access -> Generate Keys.\n    username = api_key; password = api_secret\n    [More info](https://frappe.io/docs/user/en/guides/integration/token_based_auth)\n  sources:\n  - openapi/openapi.yaml\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /method/frappe.integrations.oauth2.authorize\n    tokenUrl: /method/frappe.integrations.oauth2.get_token\n    scopes: 1\n  description:\
  \ \"This API uses OAuth 2 with the authorization code flow. \\n[More info]https://frappe.io/docs/user/en/guides/integration/using_oauth)\"\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erpnext/refs/heads/main/authentication/erpnext-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- ERP
- Enterprise Resource Planning
- Accounting
- Inventory
- Manufacturing
- Sales
- CRM
- HR
- Open Source
---
