---
api_key_in: []
api_specs:
- filename: microsoft-power-automate-management-api.yaml
  format: yaml
  label: Power Automate Management API
  slug: power-automate-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/openapi/microsoft-power-automate-management-api.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Microsoft Power Automate Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Power Automate secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Power Automate
provider_slug: microsoft-power-automate
scheme_count: 1
schemes:
- description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/token
  name: oauth2
  sources:
  - openapi/microsoft-power-automate-management-api.yaml
  type: oauth2
slug: microsoft-power-automate-authentication
source_filename: microsoft-power-automate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/microsoft-power-automate-management-api.yaml\ndocs: https://learn.microsoft.com/en-us/power-automate/web-api#authentication\noidc_discovery: well-known/microsoft-power-automate-openid-configuration.json\nnotes: >-\n  Authentication is Microsoft Entra ID (Azure AD) OAuth 2.0. The API is a\n  protected resource (https://service.flow.microsoft.com); clients acquire a\n  token via the authorization code flow and present it as a Bearer token.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/token\n    scopes: 1\n  description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.\n  sources:\n  - openapi/microsoft-power-automate-management-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/authentication/microsoft-power-automate-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Automation
- Business Process
- Integration
- Low-Code
- Microsoft
- Power Platform
- RPA
- Workflow
---
