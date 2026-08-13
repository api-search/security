---
api_key_in: []
api_specs:
- filename: cosmoplat-iot-platform-openapi.yml
  format: yaml
  label: COSMOPlat IoT Platform OpenAPI
  slug: cosmoplat-iot-platform-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmoplat/refs/heads/main/openapi/cosmoplat-iot-platform-openapi.yml
- filename: cosmoplat-iot-telemetry-asyncapi.yml
  format: yaml
  label: COSMOPlat IoT Telemetry (MQTT)
  slug: cosmoplat-iot-telemetry-mqtt
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmoplat/refs/heads/main/asyncapi/cosmoplat-iot-telemetry-asyncapi.yml
auth_types:
- userPassword
- deviceToken
description: ''
kind: authentication
layout: security
method: searched
name: Cosmoplat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cosmoplat secures its APIs with userPassword and deviceToken across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cosmoplat
provider_slug: cosmoplat
scheme_count: 3
schemes:
- applies_to: iot-mqtt.cosmoplat.com:11883 (tenant telemetry subscription)
  issued_at: 企业中心 (enterprise center) after signing in to the IoT platform
  name: enterpriseCredentials
  password: 企业密钥 — the enterprise secret
  prerequisite: The transport component (传输组件) must first be activated by the platform system administrator.
  source: https://www.cosmoplat.com/help/detail/304/1064
  surface: mqtt
  type: userPassword
  username: 企业ID — the enterprise (tenant) ID
- applies_to: iot.cosmoplat.com:1883 (device telemetry ingest)
  credential_field: Device.deviceCredentialsId (访问令牌 — access token), returned on getTenantDevicesnew and getDeviceInfoByDeviceId
  credential_types:
  - ACCESS_TOKEN
  - X509_CERTIFICATE
  - MQTT_BASIC
  name: deviceCredentials
  source: https://www.cosmoplat.com/help/detail/304/1038
  surface: mqtt
  type: deviceToken
- applies_to: https://tianyun.cosmoplat.com/ (天云控制台 — Tianyun console)
  name: consoleLogin
  note: The platform documents two tenant onboarding routes — a tenant provisioned by the IoT platform administrator, or a 卡奥斯天云 (CUBA) tenant signing in directly. Both are human console flows; neither is described as issuing an API credential.
  source: https://www.cosmoplat.com/help/detail/304/1026
  surface: web
  type: interactive
slug: cosmoplat-authentication
source_filename: cosmoplat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://www.cosmoplat.com/help/detail/304/1038\ndocs: https://www.cosmoplat.com/help/detail/304/1064\nsummary:\n  types: [userPassword, deviceToken]\n  rest_auth_documented: false\n  api_key_in: []\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: not documented for callers (X509_CERTIFICATE is available as a DEVICE\n    credential type)\ndetail: >-\n  COSMOPlat publishes two credential models for the IoT development platform and neither\n  of them covers the REST caller. Device-side credentials and MQTT tenant credentials are\n  documented; the credential a client presents to the 26 REST operations is not.\nschemes:\n- name: enterpriseCredentials\n  type: userPassword\n  surface: mqtt\n  applies_to: iot-mqtt.cosmoplat.com:11883 (tenant telemetry subscription)\n  username: 企业ID — the enterprise (tenant) ID\n  password: 企业密钥 — the enterprise secret\n  issued_at: 企业中心 (enterprise center) after signing in to the IoT\
  \ platform\n  prerequisite: The transport component (传输组件) must first be activated by the platform\n    system administrator.\n  source: https://www.cosmoplat.com/help/detail/304/1064\n- name: deviceCredentials\n  type: deviceToken\n  surface: mqtt\n  applies_to: iot.cosmoplat.com:1883 (device telemetry ingest)\n  credential_types: [ACCESS_TOKEN, X509_CERTIFICATE, MQTT_BASIC]\n  credential_field: Device.deviceCredentialsId (访问令牌 — access token), returned on\n    getTenantDevicesnew and getDeviceInfoByDeviceId\n  source: https://www.cosmoplat.com/help/detail/304/1038\n- name: consoleLogin\n  type: interactive\n  surface: web\n  applies_to: https://tianyun.cosmoplat.com/ (天云控制台 — Tianyun console)\n  note: >-\n    The platform documents two tenant onboarding routes — a tenant provisioned by the IoT\n    platform administrator, or a 卡奥斯天云 (CUBA) tenant signing in directly. Both are human\n    console flows; neither is described as issuing an API credential.\n  source: https://www.cosmoplat.com/help/detail/304/1026\n\
  rest_api_gap:\n  documented: false\n  evidence: >-\n    All 26 operations in the published reference were transcribed on 2026-08-11. The\n    Headers tables carry Content-Type and nothing else. No Authorization header, no\n    X-Auth-Token, no apiKey query parameter, no signature scheme and no auth section\n    appears anywhere in the reference.\n  consequence: >-\n    A developer cannot call this API from the documentation alone. The onboarding path is\n    to contact the platform system administrator, which makes the REST surface effectively\n    partner-gated even though its contract is fully public.\nwell_known:\n  openid_configuration: not served (404 on www.cosmoplat.com)\n  oauth_authorization_server: not served (404 on www.cosmoplat.com)\n  see: well-known/cosmoplat-well-known.yml\ngaps:\n- id: no-rest-auth-documented\n  detail: >-\n    Publish the REST credential model — where the token comes from, which header carries\n    it, how long it lives. This is the single change that\
  \ would turn a readable contract\n    into a callable one.\n- id: no-oauth-or-oidc\n  detail: No OAuth 2.0 or OpenID Connect surface is published, and neither discovery\n    document is served.\n- id: plaintext-mqtt-only\n  detail: Credentials are passed as MQTT username/password over the documented plaintext\n    ports 1883 and 11883. No TLS port is documented for either broker.\nx-evidence:\n- url: https://www.cosmoplat.com/help/detail/304/1038\n  http_status: 200\n  fetched: '2026-08-11'\n- url: https://www.cosmoplat.com/help/detail/304/1064\n  http_status: 200\n  fetched: '2026-08-11'\n- url: https://www.cosmoplat.com/.well-known/openid-configuration\n  http_status: 404\n  fetched: '2026-08-11'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosmoplat/refs/heads/main/authentication/cosmoplat-authentication.yml
summary_line: userPassword/deviceToken · 3 schemes
tags:
- Company
- Industrial Internet
- Industrial IoT
- Internet of Things
- Manufacturing
- Smart Factory
- Device Management
- Digital Transformation
- MQTT
- Telemetry
- China
---
