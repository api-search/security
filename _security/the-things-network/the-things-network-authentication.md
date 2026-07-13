---
api_key_in:
- header
api_specs:
- filename: the-things-stack-identity-server-openapi.yml
  format: yaml
  label: The Things Stack Identity Server
  slug: the-things-stack-identity-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-identity-server-openapi.yml
- filename: the-things-stack-application-server-openapi.yml
  format: yaml
  label: The Things Stack Application Server
  slug: the-things-stack-application-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-application-server-openapi.yml
- filename: the-things-stack-network-server-openapi.yml
  format: yaml
  label: The Things Stack Network Server
  slug: the-things-stack-network-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-network-server-openapi.yml
- filename: the-things-stack-gateway-server-openapi.yml
  format: yaml
  label: The Things Stack Gateway Server
  slug: the-things-stack-gateway-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-gateway-server-openapi.yml
- filename: the-things-stack-join-server-openapi.yml
  format: yaml
  label: The Things Stack Join Server
  slug: the-things-stack-join-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-join-server-openapi.yml
- filename: the-things-stack-end-device-registry-openapi.yml
  format: yaml
  label: The Things Stack End Device Registry
  slug: the-things-stack-end-device-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-end-device-registry-openapi.yml
- filename: the-things-stack-integrations-openapi.yml
  format: yaml
  label: The Things Stack Integrations
  slug: the-things-stack-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-integrations-openapi.yml
- filename: the-things-stack-packet-broker-agent-openapi.yml
  format: yaml
  label: The Things Stack Packet Broker Agent
  slug: the-things-stack-packet-broker-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-packet-broker-agent-openapi.yml
- filename: the-things-stack-events-openapi.yml
  format: yaml
  label: The Things Stack Events
  slug: the-things-stack-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-events-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: The Things Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Things Network / The Things Stack secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Things Network / The Things Stack
provider_slug: the-things-network
scheme_count: 1
schemes:
- description: 'Bearer API key. Set Authorization: Bearer NNSXS.xxxxxxxxxx.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/the-things-stack-application-server-openapi.yml
  - openapi/the-things-stack-end-device-registry-openapi.yml
  - openapi/the-things-stack-events-openapi.yml
  - openapi/the-things-stack-gateway-server-openapi.yml
  - openapi/the-things-stack-identity-server-openapi.yml
  - openapi/the-things-stack-integrations-openapi.yml
  - openapi/the-things-stack-join-server-openapi.yml
  - openapi/the-things-stack-network-server-openapi.yml
  - openapi/the-things-stack-packet-broker-agent-openapi.yml
  type: apiKey
slug: the-things-network-authentication
source_filename: the-things-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/the-things-stack-application-server-openapi.yml, openapi/the-things-stack-end-device-registry-openapi.yml,\n  openapi/the-things-stack-events-openapi.yml, openapi/the-things-stack-gateway-server-openapi.yml,\n  openapi/the-things-stack-identity-server-openapi.yml, openapi/the-things-stack-integrations-openapi.yml,\n  openapi/the-things-stack-join-server-openapi.yml, openapi/the-things-stack-network-server-openapi.yml,\n  openapi/the-things-stack-packet-broker-agent-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Bearer API key. Set Authorization: Bearer NNSXS.xxxxxxxxxx.'\n  sources:\n  - openapi/the-things-stack-application-server-openapi.yml\n  - openapi/the-things-stack-end-device-registry-openapi.yml\n  - openapi/the-things-stack-events-openapi.yml\n  - openapi/the-things-stack-gateway-server-openapi.yml\n\
  \  - openapi/the-things-stack-identity-server-openapi.yml\n  - openapi/the-things-stack-integrations-openapi.yml\n  - openapi/the-things-stack-join-server-openapi.yml\n  - openapi/the-things-stack-network-server-openapi.yml\n  - openapi/the-things-stack-packet-broker-agent-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/authentication/the-things-network-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- LoRaWAN
- IoT
- Internet Of Things
- Open Source
- Network Server
- LPWAN
- Telemetry
- Sensors
- Gateways
- Connectivity
- Apache 2.0
---
