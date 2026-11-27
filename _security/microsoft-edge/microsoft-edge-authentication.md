---
anonymous_access: true
api_key_in: []
api_specs:
- filename: microsoft-edge-browser-api-openapi.yml
  format: yaml
  label: Microsoft Edge Browser API
  slug: microsoft-edge-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-edge/openapi/microsoft-edge-browser-api-openapi.yml
- filename: microsoft-edge-packages-api-openapi.yml
  format: yaml
  label: Microsoft Edge Packages API
  slug: microsoft-edge-packages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-edge/openapi/microsoft-edge-packages-api-openapi.yml
- filename: microsoft-edge-pages-api-openapi.yml
  format: yaml
  label: Microsoft Edge Pages API
  slug: microsoft-edge-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-edge/openapi/microsoft-edge-pages-api-openapi.yml
- filename: microsoft-edge-products-api-openapi.yml
  format: yaml
  label: Microsoft Edge Products API
  slug: microsoft-edge-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-edge/openapi/microsoft-edge-products-api-openapi.yml
- filename: microsoft-edge-publishing-api-openapi.yml
  format: yaml
  label: Microsoft Edge Publishing API
  slug: microsoft-edge-publishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-edge/openapi/microsoft-edge-publishing-api-openapi.yml
- filename: microsoft-edge-targets-api-openapi.yml
  format: yaml
  label: Microsoft Edge Targets API
  slug: microsoft-edge-targets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-edge/openapi/microsoft-edge-targets-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Microsoft Edge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Edge secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Microsoft Edge
provider_slug: microsoft-edge
scheme_count: 3
schemes:
- description: 'v1.1 uses an API key. The UI in Partner Center provides API keys. Requests send "Authorization: ApiKey $ApiKey" and "X-ClientID: $ClientID".'
  header: Authorization
  headers:
  - 'Authorization: ApiKey $ApiKey'
  - 'X-ClientID: $ClientID'
  in: header
  name: apiKeyAuth
  type: apiKey
  version: v1.1
- description: v1 requires sending an access token to the API endpoint, obtained by POST to the access token URL shown in Partner Center, using Secrets. Support for v1 will end on Dec. 31, 2024.
  headers:
  - 'Authorization: Bearer $TOKEN'
  name: bearerAuth
  scheme: bearer
  status: retired
  type: http
  version: v1
- applies_to: http://localhost:9222
  description: The DevTools Protocol HTTP endpoints are served by a locally launched browser (msedge.exe --remote-debugging-port=9222); no credential is documented.
  docs: https://learn.microsoft.com/en-us/microsoft-edge/devtools/protocol/
  name: localDevTools
  type: none
slug: microsoft-edge-authentication
source_filename: microsoft-edge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://github.com/MicrosoftDocs/edge-developer/blob/main/microsoft-edge/extensions/update/api/using-addons-api.md\ndocs: https://learn.microsoft.com/en-us/microsoft-edge/extensions/update/api/using-addons-api\nsummary:\n  types:\n  - apiKey\n  - http\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  header: Authorization\n  version: v1.1\n  description: 'v1.1 uses an API key. The UI in Partner Center provides API keys. Requests send \"Authorization: ApiKey $ApiKey\" and \"X-ClientID: $ClientID\".'\n  headers:\n  - 'Authorization: ApiKey $ApiKey'\n  - 'X-ClientID: $ClientID'\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  version: v1\n  status: retired\n  description: 'v1 requires sending an access token to the API endpoint, obtained by POST to the access token URL shown in Partner Center, using Secrets. Support for v1 will end on Dec. 31, 2024.'\n  headers:\n  - 'Authorization: Bearer $TOKEN'\n- name: localDevTools\n\
  \  type: none\n  applies_to: http://localhost:9222\n  description: The DevTools Protocol HTTP endpoints are served by a locally launched browser (msedge.exe --remote-debugging-port=9222); no credential is documented.\n  docs: https://learn.microsoft.com/en-us/microsoft-edge/devtools/protocol/\n"
source_yaml_url: https://artifacts.apis.io/microsoft-edge/authentication/microsoft-edge-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Browser
- Chromium
- Developer Tools
- Edge
- Extensions
- Microsoft
- Progressive Web Apps
- Web Development
- Webview
---
