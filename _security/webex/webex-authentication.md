---
api_key_in: []
api_specs:
- filename: webex-messaging-openapi.json
  format: json
  label: Webex Messaging
  slug: messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-messaging-openapi.json
- filename: webex-meeting-openapi.json
  format: json
  label: Webex Meetings
  slug: meetings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-meeting-openapi.json
- filename: webex-admin-openapi.json
  format: json
  label: Webex Admin
  slug: admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-admin-openapi.json
- filename: webex-cloud-calling-openapi.json
  format: json
  label: Webex Cloud Calling
  slug: cloud-calling
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-cloud-calling-openapi.json
- filename: webex-contact-center-openapi.json
  format: json
  label: Webex Contact Center
  slug: contact-center
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-contact-center-openapi.json
- filename: webex-device-openapi.json
  format: json
  label: Webex Devices
  slug: devices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-device-openapi.json
- filename: webex-broadworks-openapi.json
  format: json
  label: Webex Broadworks Calling
  slug: broadworks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-broadworks-openapi.json
- filename: webex-ucm-openapi.json
  format: json
  label: Webex for UCM
  slug: ucm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-ucm-openapi.json
- filename: webex-wholesale-openapi.json
  format: json
  label: Webex Wholesale
  slug: wholesale
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-wholesale-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Webex Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Webex secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Webex
provider_slug: webex
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    scopes: 0
    tokenUrl: /
  name: oauth2
  sources:
  - openapi/webex-admin-openapi.json
  - openapi/webex-broadworks-openapi.json
  - openapi/webex-cloud-calling-openapi.json
  - openapi/webex-contact-center-openapi.json
  - openapi/webex-device-openapi.json
  - openapi/webex-meeting-openapi.json
  - openapi/webex-messaging-openapi.json
  - openapi/webex-ucm-openapi.json
  - openapi/webex-wholesale-openapi.json
  type: oauth2
- bearerFormat: JWT
  description: e.g. Bearer [example key]
  name: bearer-key
  scheme: bearer
  sources:
  - openapi/webex-admin-openapi.json
  - openapi/webex-broadworks-openapi.json
  - openapi/webex-cloud-calling-openapi.json
  - openapi/webex-contact-center-openapi.json
  - openapi/webex-device-openapi.json
  - openapi/webex-meeting-openapi.json
  - openapi/webex-messaging-openapi.json
  - openapi/webex-ucm-openapi.json
  - openapi/webex-wholesale-openapi.json
  type: http
slug: webex-authentication
source_filename: webex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/webex-admin-openapi.json, openapi/webex-broadworks-openapi.json, openapi/webex-cloud-calling-openapi.json,\n  openapi/webex-contact-center-openapi.json, openapi/webex-device-openapi.json, openapi/webex-meeting-openapi.json,\n  openapi/webex-messaging-openapi.json, openapi/webex-ucm-openapi.json, openapi/webex-wholesale-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    tokenUrl: /\n    scopes: 0\n  sources:\n  - openapi/webex-admin-openapi.json\n  - openapi/webex-broadworks-openapi.json\n  - openapi/webex-cloud-calling-openapi.json\n  - openapi/webex-contact-center-openapi.json\n  - openapi/webex-device-openapi.json\n  - openapi/webex-meeting-openapi.json\n  - openapi/webex-messaging-openapi.json\n  - openapi/webex-ucm-openapi.json\n  - openapi/webex-wholesale-openapi.json\n\
  - name: bearer-key\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: e.g. Bearer [example key]\n  sources:\n  - openapi/webex-admin-openapi.json\n  - openapi/webex-broadworks-openapi.json\n  - openapi/webex-cloud-calling-openapi.json\n  - openapi/webex-contact-center-openapi.json\n  - openapi/webex-device-openapi.json\n  - openapi/webex-meeting-openapi.json\n  - openapi/webex-messaging-openapi.json\n  - openapi/webex-ucm-openapi.json\n  - openapi/webex-wholesale-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/authentication/webex-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Calling
- Collaboration
- Communication
- Enterprise
- Messaging
- Video Conferencing
---
