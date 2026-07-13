---
api_key_in:
- header
api_specs:
- filename: reactor-api.yml
  format: yaml
  label: Adobe Launch Reactor API
  slug: adobe-launch-reactor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/reactor-api.yml
- filename: extension-api.yml
  format: yaml
  label: Adobe Launch Extension API
  slug: adobe-launch-extension-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/extension-api.yml
- filename: event-forwarding-api.yml
  format: yaml
  label: Adobe Experience Platform Event Forwarding API
  slug: adobe-experience-platform-event-forwarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/event-forwarding-api.yml
- filename: data-collection-api.yml
  format: yaml
  label: Adobe Experience Platform Data Collection API
  slug: adobe-experience-platform-data-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/data-collection-api.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Launch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adobe Launch secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adobe Launch
provider_slug: adobe-launch
scheme_count: 3
schemes:
- description: OAuth 2.0 access token for authenticated data collection via server.adobedc.net.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/data-collection-api.yml
  - openapi/event-forwarding-api.yml
  - openapi/extension-api.yml
  - openapi/reactor-api.yml
  type: http
- description: Client ID credential from Adobe Developer Console.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/data-collection-api.yml
  - openapi/event-forwarding-api.yml
  - openapi/extension-api.yml
  - openapi/reactor-api.yml
  type: apiKey
- description: Adobe Organization ID.
  in: header
  name: orgId
  parameter: x-gw-ims-org-id
  sources:
  - openapi/data-collection-api.yml
  - openapi/event-forwarding-api.yml
  - openapi/extension-api.yml
  - openapi/reactor-api.yml
  type: apiKey
slug: adobe-launch-authentication
source_filename: adobe-launch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/data-collection-api.yml, openapi/event-forwarding-api.yml, openapi/extension-api.yml,\n  openapi/reactor-api.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token for authenticated data collection via server.adobedc.net.\n  sources:\n  - openapi/data-collection-api.yml\n  - openapi/event-forwarding-api.yml\n  - openapi/extension-api.yml\n  - openapi/reactor-api.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Client ID credential from Adobe Developer Console.\n  sources:\n  - openapi/data-collection-api.yml\n  - openapi/event-forwarding-api.yml\n  - openapi/extension-api.yml\n  - openapi/reactor-api.yml\n- name: orgId\n  type: apiKey\n  in: header\n  parameter: x-gw-ims-org-id\n  description: Adobe Organization ID.\n  sources:\n  - openapi/data-collection-api.yml\n\
  \  - openapi/event-forwarding-api.yml\n  - openapi/extension-api.yml\n  - openapi/reactor-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/authentication/adobe-launch-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
---
