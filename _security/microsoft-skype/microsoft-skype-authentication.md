---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: microsoft-skype-deliveryreports-api-openapi.yml
  format: yaml
  label: Microsoft Skype Delivery Reports API
  slug: microsoft-skype-deliveryreports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-deliveryreports-api-openapi.yml
- filename: microsoft-skype-messages-api-openapi.yml
  format: yaml
  label: Microsoft Skype Messages API
  slug: microsoft-skype-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-messages-api-openapi.yml
- filename: microsoft-skype-optoutsadd-api-openapi.yml
  format: yaml
  label: Microsoft Skype Opt Outs Add API
  slug: microsoft-skype-optoutsadd-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-optoutsadd-api-openapi.yml
- filename: microsoft-skype-optoutscheck-api-openapi.yml
  format: yaml
  label: Microsoft Skype Opt Outs Check API
  slug: microsoft-skype-optoutscheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-optoutscheck-api-openapi.yml
- filename: microsoft-skype-optoutsremove-api-openapi.yml
  format: yaml
  label: Microsoft Skype Opt Outs Remove API
  slug: microsoft-skype-optoutsremove-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-optoutsremove-api-openapi.yml
- filename: microsoft-skype-participants-api-openapi.yml
  format: yaml
  label: Microsoft Skype Participants API
  slug: microsoft-skype-participants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-participants-api-openapi.yml
- filename: microsoft-skype-sms-api-openapi.yml
  format: yaml
  label: Microsoft Skype Sms API
  slug: microsoft-skype-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-sms-api-openapi.yml
- filename: microsoft-skype-threads-api-openapi.yml
  format: yaml
  label: Microsoft Skype Threads API
  slug: microsoft-skype-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-threads-api-openapi.yml
- filename: microsoft-skype-typingnotifications-api-openapi.yml
  format: yaml
  label: Microsoft Skype Typing Notifications API
  slug: microsoft-skype-typingnotifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-typingnotifications-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Microsoft Skype Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Microsoft Skype secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Microsoft Skype
provider_slug: microsoft-skype
scheme_count: 2
schemes:
- description: An ACS (Azure Communication Services) user access token.
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/microsoft-skype-chat-openapi.yml
  type: apiKey
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-skype-sms-openapi.yml
  type: oauth2
slug: microsoft-skype-authentication
source_filename: microsoft-skype-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/microsoft-skype-chat-openapi.yml, openapi/microsoft-skype-sms-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - implicit\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: An ACS (Azure Communication Services) user access token.\n  sources:\n  - openapi/microsoft-skype-chat-openapi.yml\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow\n  sources:\n  - openapi/microsoft-skype-sms-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-skype/authentication/microsoft-skype-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Communications
- Messaging
- Microsoft
- Video
- Voice
---
