---
api_key_in:
- header
api_specs:
- filename: china-mobile-onenet-studio-openapi.yml
  format: yaml
  label: OneNET Studio Application API
  slug: onenet-studio-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/china-mobile/refs/heads/main/openapi/china-mobile-onenet-studio-openapi.yml
- filename: china-mobile-vcs-openapi.yml
  format: yaml
  label: OneNET Voice Call Service (VCS) API
  slug: onenet-voice-call-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/china-mobile/refs/heads/main/openapi/china-mobile-vcs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: China Mobile Authentication
name_suffix: Authentication
oauth_flows: []
overview: China Mobile secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: China Mobile
provider_slug: china-mobile
scheme_count: 2
schemes:
- description: 'OneNET signed authorization token: version=2020-05-29&res=userid/{userid}&et={epoch}&method={md5|sha1|sha256}&sign={signature}, where sign = base64(hmac_method(base64decode(accessKey), et + "\n" + method + "\n" + res + "\n" + version)). Reference: https://open.iot.10086.cn/doc/iot_platform/book/api/auth.html'
  in: header
  name: onenetAuthorization
  parameter: authorization
  sources:
  - openapi/china-mobile-onenet-studio-openapi.yml
  type: apiKey
- description: 'OneNET signed authorization token: `version=2020-05-29&res=userid/{userid}&et={epoch}&method={md5|sha1|sha256}&sign={signature}` where sign = base64(hmac_method(base64decode(accessKey), et + "\n" + method + "\n" + res + "\n" + version)). See https://open.iot.10086.cn/doc/iot_platform/book/api/auth.html'
  in: header
  name: onenetAuthorization
  parameter: Authorization
  sources:
  - openapi/china-mobile-vcs-openapi.yml
  type: apiKey
slug: china-mobile-authentication
source_filename: china-mobile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: derived\nsource: openapi/china-mobile-onenet-studio-openapi.yml, openapi/china-mobile-vcs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: onenetAuthorization\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: 'OneNET signed authorization token: version=2020-05-29&res=userid/{userid}&et={epoch}&method={md5|sha1|sha256}&sign={signature},\n    where sign = base64(hmac_method(base64decode(accessKey), et + \"\\n\" + method + \"\\n\" + res\n    + \"\\n\" + version)). Reference: https://open.iot.10086.cn/doc/iot_platform/book/api/auth.html'\n  sources:\n  - openapi/china-mobile-onenet-studio-openapi.yml\n- name: onenetAuthorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'OneNET signed authorization token: `version=2020-05-29&res=userid/{userid}&et={epoch}&method={md5|sha1|sha256}&sign={signature}`\n    where sign = base64(hmac_method(base64decode(accessKey),\
  \ et + \"\\n\" + method + \"\\n\" + res\n    + \"\\n\" + version)). See https://open.iot.10086.cn/doc/iot_platform/book/api/auth.html'\n  sources:\n  - openapi/china-mobile-vcs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/china-mobile/refs/heads/main/authentication/china-mobile-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Telecommunications
- China
- Mobile Network Operator
- Network APIs
- CAMARA
- GSMA Open Gateway
- IoT
- 5G
- Broadband
- Quality on Demand
- Number Authentication
- Satellite
---
