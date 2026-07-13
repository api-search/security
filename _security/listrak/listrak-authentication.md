---
api_key_in:
- header
api_specs:
- filename: listrak-email-openapi.yml
  format: yaml
  label: Listrak Email REST API
  slug: email
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-email-openapi.yml
- filename: listrak-sms-openapi.yml
  format: yaml
  label: Listrak SMS REST API
  slug: sms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-sms-openapi.yml
- filename: listrak-crosschannel-openapi.yml
  format: yaml
  label: Listrak Cross Channel REST API
  slug: crosschannel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-crosschannel-openapi.yml
- filename: listrak-data-openapi.yml
  format: yaml
  label: Listrak Data Import REST API
  slug: data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-data-openapi.yml
- filename: listrak-twowaysms-openapi.yml
  format: yaml
  label: Listrak Two-Way SMS Conversation REST API
  slug: twowaysms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-twowaysms-openapi.yml
- filename: listrak-mobileclient-openapi.yml
  format: yaml
  label: Listrak Mobile App Push API
  slug: mobileclient
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-mobileclient-openapi.yml
- filename: listrak-privacy-openapi.yml
  format: yaml
  label: Listrak Privacy REST API
  slug: privacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-privacy-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Listrak Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Listrak secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Listrak
provider_slug: listrak
scheme_count: 3
schemes:
- in: header
  name: Authorizer
  parameter: Authorization
  sources:
  - openapi/listrak-crosschannel-openapi.yml
  - openapi/listrak-twowaysms-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.listrak.com/OAuth2/Token
  name: OAuth2
  sources:
  - openapi/listrak-data-openapi.yml
  - openapi/listrak-email-openapi.yml
  - openapi/listrak-privacy-openapi.yml
  - openapi/listrak-sms-openapi.yml
  type: oauth2
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/listrak-mobileclient-openapi.yml
  type: apiKey
slug: listrak-authentication
source_filename: listrak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/listrak-crosschannel-openapi.yml, openapi/listrak-data-openapi.yml, openapi/listrak-email-openapi.yml,\n  openapi/listrak-mobileclient-openapi.yml, openapi/listrak-privacy-openapi.yml, openapi/listrak-sms-openapi.yml,\n  openapi/listrak-twowaysms-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Authorizer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/listrak-crosschannel-openapi.yml\n  - openapi/listrak-twowaysms-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.listrak.com/OAuth2/Token\n    scopes: 0\n  sources:\n  - openapi/listrak-data-openapi.yml\n  - openapi/listrak-email-openapi.yml\n  - openapi/listrak-privacy-openapi.yml\n  - openapi/listrak-sms-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n\
  \  sources:\n  - openapi/listrak-mobileclient-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/authentication/listrak-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Email Marketing
- SMS Marketing
- Marketing Automation
- Cross-Channel
- Retail
- Push Notifications
- Data Import
- Privacy
---
