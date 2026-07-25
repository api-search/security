---
api_key_in:
- header
api_specs:
- filename: adobe-launch-builds-api-openapi.yml
  format: yaml
  label: Adobe Launch Builds API
  slug: adobe-launch-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-builds-api-openapi.yml
- filename: adobe-launch-callbacks-api-openapi.yml
  format: yaml
  label: Adobe Launch Callbacks API
  slug: adobe-launch-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-callbacks-api-openapi.yml
- filename: adobe-launch-companies-api-openapi.yml
  format: yaml
  label: Adobe Launch Companies API
  slug: adobe-launch-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-companies-api-openapi.yml
- filename: adobe-launch-data-elements-api-openapi.yml
  format: yaml
  label: Adobe Launch Data Elements API
  slug: adobe-launch-data-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-data-elements-api-openapi.yml
- filename: adobe-launch-edge-network-api-api-openapi.yml
  format: yaml
  label: Adobe Launch Edge Network API API
  slug: adobe-launch-edge-network-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-edge-network-api-api-openapi.yml
- filename: adobe-launch-environments-api-openapi.yml
  format: yaml
  label: Adobe Launch Environments API
  slug: adobe-launch-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-environments-api-openapi.yml
- filename: adobe-launch-extension-packages-api-openapi.yml
  format: yaml
  label: Adobe Launch Extension Packages API
  slug: adobe-launch-extension-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-extension-packages-api-openapi.yml
- filename: adobe-launch-extensions-api-openapi.yml
  format: yaml
  label: Adobe Launch Extensions API
  slug: adobe-launch-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-extensions-api-openapi.yml
- filename: adobe-launch-hosts-api-openapi.yml
  format: yaml
  label: Adobe Launch Hosts API
  slug: adobe-launch-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-hosts-api-openapi.yml
- filename: adobe-launch-libraries-api-openapi.yml
  format: yaml
  label: Adobe Launch Libraries API
  slug: adobe-launch-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-libraries-api-openapi.yml
- filename: adobe-launch-media-edge-api-api-openapi.yml
  format: yaml
  label: Adobe Launch Media Edge API API
  slug: adobe-launch-media-edge-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-media-edge-api-api-openapi.yml
- filename: adobe-launch-properties-api-openapi.yml
  format: yaml
  label: Adobe Launch Properties API
  slug: adobe-launch-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-properties-api-openapi.yml
- filename: adobe-launch-rule-components-api-openapi.yml
  format: yaml
  label: Adobe Launch Rule Components API
  slug: adobe-launch-rule-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-rule-components-api-openapi.yml
- filename: adobe-launch-rules-api-openapi.yml
  format: yaml
  label: Adobe Launch Rules API
  slug: adobe-launch-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-rules-api-openapi.yml
- filename: adobe-launch-search-api-openapi.yml
  format: yaml
  label: Adobe Launch Search API
  slug: adobe-launch-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-search-api-openapi.yml
- filename: adobe-launch-secrets-api-openapi.yml
  format: yaml
  label: Adobe Launch Secrets API
  slug: adobe-launch-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/openapi/adobe-launch-secrets-api-openapi.yml
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
