---
api_key_in:
- query
- body
api_specs:
- filename: leanplum-a-b-tests-api-openapi.yml
  format: yaml
  label: Leanplum A/B Tests API
  slug: leanplum-a-b-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-a-b-tests-api-openapi.yml
- filename: leanplum-content-variables-api-openapi.yml
  format: yaml
  label: Leanplum Content & Variables API
  slug: leanplum-content-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-content-variables-api-openapi.yml
- filename: leanplum-data-export-api-openapi.yml
  format: yaml
  label: Leanplum Data Export API
  slug: leanplum-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-data-export-api-openapi.yml
- filename: leanplum-events-tracking-api-openapi.yml
  format: yaml
  label: Leanplum Events & Tracking API
  slug: leanplum-events-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-events-tracking-api-openapi.yml
- filename: leanplum-messaging-api-openapi.yml
  format: yaml
  label: Leanplum Messaging API
  slug: leanplum-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-messaging-api-openapi.yml
- filename: leanplum-postbacks-batch-api-openapi.yml
  format: yaml
  label: Leanplum Postbacks & Batch API
  slug: leanplum-postbacks-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-postbacks-batch-api-openapi.yml
- filename: leanplum-user-device-attributes-api-openapi.yml
  format: yaml
  label: Leanplum User & Device Attributes API
  slug: leanplum-user-device-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-user-device-attributes-api-openapi.yml
- filename: leanplum-campaigns-api-openapi.yml
  format: yaml
  label: Leanplum Campaigns API
  slug: leanplum-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-campaigns-api-openapi.yml
- filename: leanplum-export-data-api-openapi.yml
  format: yaml
  label: Leanplum Export Data API
  slug: leanplum-export-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-export-data-api-openapi.yml
- filename: leanplum-files-and-variables-api-openapi.yml
  format: yaml
  label: Leanplum Files and Variables API
  slug: leanplum-files-and-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-files-and-variables-api-openapi.yml
- filename: leanplum-import-data-api-openapi.yml
  format: yaml
  label: Leanplum Import Data API
  slug: leanplum-import-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-import-data-api-openapi.yml
- filename: leanplum-messages-api-openapi.yml
  format: yaml
  label: Leanplum Messages API
  slug: leanplum-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-messages-api-openapi.yml
- filename: leanplum-user-behavior-api-openapi.yml
  format: yaml
  label: Leanplum User Behavior API
  slug: leanplum-user-behavior-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-user-behavior-api-openapi.yml
- filename: leanplum-user-information-api-openapi.yml
  format: yaml
  label: Leanplum User Information API
  slug: leanplum-user-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-user-information-api-openapi.yml
auth_types:
- apiKey
description: Leanplum authenticates every request with two API-key parameters carried in the query string or the request body — an `appId` identifying the Leanplum app, and a `clientKey` whose CLASS determines which methods you may call. There is no OAuth, no OIDC, no bearer token, no signature scheme, and no Authorization header. Keys are long-lived and are read from the dashboard.
kind: authentication
layout: security
method: searched
name: Leanplum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leanplum secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Leanplum
provider_slug: leanplum
scheme_count: 2
schemes:
- description: The application ID. Found in the Leanplum dashboard under Development -> App Settings -> API Keys.
  in: query
  name: appIdQuery
  parameter: appId
  required: true
  sources:
  - openapi/leanplum-api-openapi.json
  - https://docs.leanplum.com/docs/use-the-right-api-keys
  type: apiKey
- description: The client access key. Must be the production, development, read-only, or data export key, depending on which API method you are calling.
  in: query
  name: clientKeyQuery
  parameter: clientKey
  required: true
  sources:
  - openapi/leanplum-api-openapi.json
  - https://docs.leanplum.com/docs/use-the-right-api-keys
  type: apiKey
slug: leanplum-authentication
source_filename: leanplum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/leanplum-api-openapi.json\ndocs: https://docs.leanplum.com/docs/use-the-right-api-keys\nadditional_docs:\n- https://docs.leanplum.com/reference/making-requests\n- https://docs.leanplum.com/reference/api-methods\n- https://docs.leanplum.com/reference/responses\ndescription: >-\n  Leanplum authenticates every request with two API-key parameters carried in the\n  query string or the request body — an `appId` identifying the Leanplum app, and a\n  `clientKey` whose CLASS determines which methods you may call. There is no OAuth,\n  no OIDC, no bearer token, no signature scheme, and no Authorization header. Keys\n  are long-lived and are read from the dashboard.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - body\n  oauth: false\n  oidc: false\n  mtls: false\n  bearer: false\n  authorization_header: false\nschemes:\n- name: appIdQuery\n  type: apiKey\n  in: query\n  parameter: appId\n  required: true\n  description:\
  \ >-\n    The application ID. Found in the Leanplum dashboard under Development -> App\n    Settings -> API Keys.\n  sources:\n  - openapi/leanplum-api-openapi.json\n  - https://docs.leanplum.com/docs/use-the-right-api-keys\n- name: clientKeyQuery\n  type: apiKey\n  in: query\n  parameter: clientKey\n  required: true\n  description: >-\n    The client access key. Must be the production, development, read-only, or data\n    export key, depending on which API method you are calling.\n  sources:\n  - openapi/leanplum-api-openapi.json\n  - https://docs.leanplum.com/docs/use-the-right-api-keys\nkey_classes:\n- id: production\n  purpose: Live write methods against the production pipeline.\n  methods: [start, stop, track, advance, pauseSession, resumeSession, pauseState,\n    resumeState, heartbeat, setUserAttributes, setDeviceAttributes, setTrafficSourceInfo,\n    sendMessage, getVars, downloadFile, getAndroidNotificationChannels]\n- id: development\n  purpose: >-\n    Test/development pipeline\
  \ and content-mutating methods. Sends data in real time\n    over an open socket and keeps activity out of Analytics.\n  methods: [registerDevice, deleteUser, setVars, deleteVars, uploadFile,\n    addAndroidNotificationChannel, deleteAndroidNotificationChannel, multi,\n    getMultiResults, startCampaign]\n  warning: >-\n    Never ship a development key in a production build — the open socket degrades app\n    performance and the data is not captured in analytics.\n- id: data export\n  purpose: Data egress and postback rule management.\n  methods: [exportData, exportReport, exportUser, exportUsers, getExportResults,\n    addPostback, listPostbacks, deletePostback]\n- id: content read-only\n  purpose: Read dashboard-authored content.\n  methods: [getMessage, getMessages, getUnsubscribeCategories, getAbTest, getAbTests, getVariant]\n- id: content read-write\n  purpose: >-\n    Read and write dashboard content. Present as `contentReadWriteKey` in Leanplum's\n    own published Postman environment.\n\
  key_management:\n  discovery_path: Leanplum dashboard -> Development -> App Settings -> API Keys\n  discovery_url: https://www.leanplum.com/dashboard#/account/apps\n  environments: >-\n    Leanplum provisions TWO apps per customer — one development, one production —\n    each with its own key set, specifically to reduce the risk of using the wrong key.\n  rotation_policy: not published\n  expiry: none published (keys are long-lived)\n  scopes: none — authorization is by key class, not by scope\ntransport_security:\n  https_required: true\n  note: >-\n    The published spec lists both `https://api.leanplum.com` and\n    `http://api.leanplum.com` as servers. Use HTTPS only — credentials travel in the\n    query string, so a plaintext call leaks the clientKey to every intermediary.\nrisks:\n- >-\n    Credentials in the QUERY STRING are logged by proxies, CDNs, browser history and\n    server access logs by default. Prefer POST with the arguments in the JSON body,\n    which Leanplum explicitly\
  \ supports, over GET.\n- >-\n    No scopes and no per-key expiry: a leaked production key can write to every live\n    profile in the app until it is rotated from the dashboard.\nfailure_modes:\n- message: Invalid access key\n  cause: Wrong key class for the method, or a mismatched appId/clientKey pair.\n  see: errors/leanplum-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/authentication/leanplum-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Mobile Marketing
- Customer Engagement
- Push Notifications
- Messaging
- A/B Testing
- Analytics
- CleverTap
---
