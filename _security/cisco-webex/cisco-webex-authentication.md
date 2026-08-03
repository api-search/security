---
api_key_in: []
api_specs:
- filename: cisco-webex-admin-openapi.json
  format: json
  label: Cisco Webex Administration API
  slug: admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-admin-openapi.json
- filename: cisco-webex-broadworks-openapi.json
  format: json
  label: Cisco Webex BroadWorks API
  slug: broadworks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-broadworks-openapi.json
- filename: cisco-webex-cloud-calling-openapi.json
  format: json
  label: Cisco Webex Cloud Calling API
  slug: cloud-calling
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-cloud-calling-openapi.json
- filename: cisco-webex-contact-center-openapi.json
  format: json
  label: Cisco Webex Contact Center API
  slug: contact-center
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-contact-center-openapi.json
- filename: cisco-webex-device-openapi.json
  format: json
  label: Cisco Webex Devices API
  slug: device
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-device-openapi.json
- filename: cisco-webex-meeting-openapi.json
  format: json
  label: Cisco Webex Meetings API
  slug: meeting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-meeting-openapi.json
- filename: cisco-webex-messaging-openapi.json
  format: json
  label: Cisco Webex Messaging API
  slug: messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-messaging-openapi.json
- filename: cisco-webex-ucm-openapi.json
  format: json
  label: Cisco Webex Unified CM API
  slug: ucm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-ucm-openapi.json
- filename: cisco-webex-wholesale-openapi.json
  format: json
  label: Cisco Webex Wholesale API
  slug: wholesale
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-wholesale-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cisco Webex Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cisco Webex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cisco Webex
provider_slug: cisco-webex
scheme_count: 1
schemes:
- description: Webex API access token supplied in the Authorization header. Obtain via the OAuth 2.0 authorization-code flow, a Personal Access Token, a Service App, or a Bot token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cisco-webex-admin-openapi.json
  - openapi/cisco-webex-messaging-openapi.json
  - openapi/cisco-webex-cloud-calling-openapi.json
  - openapi/cisco-webex-meeting-openapi.json
  - openapi/cisco-webex-device-openapi.json
  - openapi/cisco-webex-messaging-openapi.json
  - openapi/cisco-webex-admin-openapi.json
  - openapi/cisco-webex-meeting-openapi.json
  - openapi/cisco-webex-messaging-openapi.json
  - openapi/cisco-webex-messaging-openapi.json
  - openapi/cisco-webex-admin-openapi.json
  - openapi/cisco-webex-messaging-openapi.json
  - openapi/cisco-webex-meeting-openapi.json
  - openapi/cisco-webex-admin-openapi.json
  - openapi/cisco-webex-messaging-openapi.json
  - openapi/cisco-webex-messaging-openapi.json
  - openapi/cisco-webex-messaging-openapi.json
  - openapi/cisco-webex-messaging-openapi.json
  - openapi/cisco-webex-admin-openapi.json
  type: http
slug: cisco-webex-authentication
source_filename: cisco-webex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: >-\n  https://developer.webex.com/docs/getting-started#authentication and\n  https://developer.webex.com/docs/integrations — upgraded from the OpenAPI-\n  derived profile with the documented Webex token model. All 19 captured specs\n  declare a single http bearer scheme (bearerAuth); Webex issues that bearer\n  token through four documented mechanisms.\ndocs: https://developer.webex.com/docs/getting-started#authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\ntoken_mechanisms:\n  - name: OAuth 2.0 Integration\n    for: Apps acting on behalf of a Webex user (authorization-code flow).\n    authorizationUrl: https://webexapis.com/v1/authorize\n    tokenUrl: https://webexapis.com/v1/access_token\n    scopes: scopes/cisco-webex-scopes.yml\n  - name: Personal Access Token\n    for: Interactive developer testing on your own account (~12h lifetime).\n  - name: Service App\n\
  \    for: >-\n      Server-to-server integrations authorized org-wide by an admin; long-lived,\n      admin-scoped tokens (see blog \"Service App token management\").\n  - name: Bot\n    for: A bot account with a fixed access token for messaging/webhook automations.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Webex API access token supplied in the Authorization header. Obtain via the\n    OAuth 2.0 authorization-code flow, a Personal Access Token, a Service App, or\n    a Bot token.\n  sources:\n  - openapi/cisco-webex-admin-openapi.json\n  - openapi/cisco-webex-messaging-openapi.json\n  - openapi/cisco-webex-cloud-calling-openapi.json\n  - openapi/cisco-webex-meeting-openapi.json\n  - openapi/cisco-webex-device-openapi.json\n  - openapi/cisco-webex-messaging-openapi.json\n  - openapi/cisco-webex-admin-openapi.json\n  - openapi/cisco-webex-meeting-openapi.json\n  - openapi/cisco-webex-messaging-openapi.json\n  - openapi/cisco-webex-messaging-openapi.json\n\
  \  - openapi/cisco-webex-admin-openapi.json\n  - openapi/cisco-webex-messaging-openapi.json\n  - openapi/cisco-webex-meeting-openapi.json\n  - openapi/cisco-webex-admin-openapi.json\n  - openapi/cisco-webex-messaging-openapi.json\n  - openapi/cisco-webex-messaging-openapi.json\n  - openapi/cisco-webex-messaging-openapi.json\n  - openapi/cisco-webex-messaging-openapi.json\n  - openapi/cisco-webex-admin-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/authentication/cisco-webex-authentication.yml
summary_line: http · 1 scheme
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
---
