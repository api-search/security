---
api_key_in:
- header
api_specs:
- filename: wealthbox-openapi.yml
  format: yaml
  label: Wealthbox CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/openapi/wealthbox-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wealthbox Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wealthbox secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wealthbox
provider_slug: wealthbox
scheme_count: 2
schemes:
- description: Personal Access Token issued from the Wealthbox account settings.
  in: header
  name: accessToken
  parameter: ACCESS_TOKEN
  sources:
  - openapi/wealthbox-openapi.yml
  type: apiKey
- description: OAuth 2.0 authorization code flow for third-party integrations.
  flows:
  - authorizationUrl: https://app.crmworkspace.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://app.crmworkspace.com/oauth/token
  name: oauth2
  sources:
  - openapi/wealthbox-openapi.yml
  type: oauth2
slug: wealthbox-authentication
source_filename: wealthbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wealthbox-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: ACCESS_TOKEN\n  description: Personal Access Token issued from the Wealthbox account settings.\n  sources:\n  - openapi/wealthbox-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.crmworkspace.com/oauth/authorize\n    tokenUrl: https://app.crmworkspace.com/oauth/token\n    scopes: 2\n  description: OAuth 2.0 authorization code flow for third-party integrations.\n  sources:\n  - openapi/wealthbox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/authentication/wealthbox-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- CRM
- Financial Advisors
- Wealth Management
- Contact Management
- Workflow Automation
- SaaS
---
