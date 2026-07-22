---
api_key_in:
- header
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Medigate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Medigate secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Medigate
provider_slug: medigate
scheme_count: 2
schemes:
- api_version: v1
  description: Medigate API V1 authenticates with the console username and password over HTTPS to api.medigate.io.
  name: MedigateBasicV1
  scheme: basic
  sources:
  - https://docs.axonius.com/docs/medigate
  type: http
- api_version: v2
  description: Medigate API V2 authenticates with an API token generated inside the Medigate management console and presented on requests to api.medigate.io. Integrations use it to pull the Device List, Device Groups, and device Risk scores.
  in: header
  name: MedigateApiTokenV2
  sources:
  - https://docs.axonius.com/docs/medigate
  - https://library.humio.com/integrations/integrations-medigate.html
  type: apiKey
slug: medigate-authentication
source_filename: medigate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.axonius.com/docs/medigate\ndocs: https://docs.axonius.com/docs/medigate\nnote: >-\n  Medigate (now Claroty) exposes a customer-facing REST API for its healthcare\n  device-security platform at api.medigate.io. The interactive API reference at\n  https://api.medigate.io/docs is password-gated (\"Contact support to get a\n  password for the documentation\") so no public OpenAPI is available; the auth\n  model below is reconstructed from published third-party integration guides\n  (Axonius, CrowdStrike LogScale) that document how to connect to the Medigate\n  API. Two versions are documented: V1 (HTTP basic username/password) and V2\n  (API token generated in the Medigate management console).\nhost: api.medigate.io\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: MedigateBasicV1\n  type: http\n  scheme: basic\n  api_version: v1\n  description: >-\n    Medigate\
  \ API V1 authenticates with the console username and password over\n    HTTPS to api.medigate.io.\n  sources:\n  - https://docs.axonius.com/docs/medigate\n- name: MedigateApiTokenV2\n  type: apiKey\n  in: header\n  api_version: v2\n  description: >-\n    Medigate API V2 authenticates with an API token generated inside the\n    Medigate management console and presented on requests to api.medigate.io.\n    Integrations use it to pull the Device List, Device Groups, and device\n    Risk scores.\n  sources:\n  - https://docs.axonius.com/docs/medigate\n  - https://library.humio.com/integrations/integrations-medigate.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medigate/refs/heads/main/authentication/medigate-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Infrastructure Saas
- Cybersecurity
- Healthcare
- Medical Devices
- Internet of Things
- Device Security
- Network Security
---
