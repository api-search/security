---
api_key_in:
- header
- query
api_specs:
- filename: screenleap-inc-screen-sharing-openapi.yml
  format: yaml
  label: Screenleap Screen Sharing API
  slug: screenleap-screen-sharing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenleap-inc/refs/heads/main/openapi/screenleap-inc-screen-sharing-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Screenleap Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Screenleap Inc secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Screenleap Inc
provider_slug: screenleap-inc
scheme_count: 2
schemes:
- also_accepts_query: true
  description: Account identifier chosen when creating the developer account.
  in: header
  name: accountId
  parameter: accountid
  sources:
  - openapi/screenleap-inc-screen-sharing-openapi.yml
  type: apiKey
- description: Secret authentication token issued with the developer account, retrievable from the Developer page under the Account menu.
  in: header
  name: authToken
  parameter: authtoken
  sources:
  - openapi/screenleap-inc-screen-sharing-openapi.yml
  type: apiKey
slug: screenleap-inc-authentication
source_filename: screenleap-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: \"2026-07-21\"\nmethod: searched\nsource: https://www.screenleap.com/api/native/doc/http-calls\ndocs: https://www.screenleap.com/api/native/quick-start\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  notes: >-\n    Every request must carry an accountid (chosen at developer-account signup)\n    and a secret authtoken. Both are sent as request headers; accountid may\n    alternatively be supplied as a query-string parameter. There is no OAuth,\n    OIDC or per-scope model.\nschemes:\n  - name: accountId\n    type: apiKey\n    in: header\n    parameter: accountid\n    also_accepts_query: true\n    description: Account identifier chosen when creating the developer account.\n    sources: [openapi/screenleap-inc-screen-sharing-openapi.yml]\n  - name: authToken\n    type: apiKey\n    in: header\n    parameter: authtoken\n    description: Secret authentication token issued with the developer account, retrievable from the Developer page\
  \ under the Account menu.\n    sources: [openapi/screenleap-inc-screen-sharing-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/screenleap-inc/refs/heads/main/authentication/screenleap-inc-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Screen Sharing
- Video Conferencing
- Collaboration
- Real-Time Communication
- WebRTC
- Embedded
- Developer Tools
---
