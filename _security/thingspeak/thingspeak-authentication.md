---
api_key_in:
- header
- query
api_specs:
- filename: thingspeak-channels-api-openapi.yml
  format: yaml
  label: ThingSpeak Channels API
  slug: thingspeak-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/openapi/thingspeak-channels-api-openapi.yml
- filename: thingspeak-feeds-api-openapi.yml
  format: yaml
  label: ThingSpeak Feeds API
  slug: thingspeak-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/openapi/thingspeak-feeds-api-openapi.yml
- filename: thingspeak-update-api-openapi.yml
  format: yaml
  label: ThingSpeak Update API
  slug: thingspeak-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/openapi/thingspeak-update-api-openapi.yml
- filename: thingspeak-mqtt-asyncapi.yml
  format: yaml
  label: ThingSpeak MQTT API
  slug: thingspeak-mqtt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/asyncapi/thingspeak-mqtt-asyncapi.yml
- filename: thingspeak-talkback-api-openapi.yml
  format: yaml
  label: ThingSpeak TalkBack API
  slug: thingspeak-talkback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/openapi/thingspeak-talkback-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Thingspeak Authentication
name_suffix: Authentication
oauth_flows: []
overview: ThingSpeak secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ThingSpeak
provider_slug: thingspeak
scheme_count: 2
schemes:
- in: header
  name: UserApiKeyHeader
  parameter: THINGSPEAKAPIKEY
  sources:
  - openapi/thingspeak-channels-api-openapi.yml
  - openapi/thingspeak-update-api-openapi.yml
  type: apiKey
- in: query
  name: TalkBackKeyQuery
  parameter: api_key
  sources:
  - openapi/thingspeak-talkback-api-openapi.yml
  - openapi/thingspeak-update-api-openapi.yml
  type: apiKey
slug: thingspeak-authentication
source_filename: thingspeak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thingspeak-channels-api-openapi.yml, openapi/thingspeak-talkback-api-openapi.yml,\n  openapi/thingspeak-update-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: UserApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: THINGSPEAKAPIKEY\n  sources:\n  - openapi/thingspeak-channels-api-openapi.yml\n  - openapi/thingspeak-update-api-openapi.yml\n- name: TalkBackKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/thingspeak-talkback-api-openapi.yml\n  - openapi/thingspeak-update-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/authentication/thingspeak-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- IoT
- Internet of Things
- Analytics
- Time Series
- MQTT
- MATLAB
- Sensors
- Telemetry
---
