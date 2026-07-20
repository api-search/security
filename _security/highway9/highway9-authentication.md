---
api_key_in:
- header
auth_types:
- apiKey
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Highway9 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Highway9 secures its APIs with apiKey and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Highway9
provider_slug: highway9
scheme_count: 2
schemes:
- description: API token credential managed via the apiToken resource. Tokens are issued to signed partners through the Mobile Center partner portal and presented on API requests to the orchestration endpoint.
  in: header
  name: apiToken
  sources:
  - docs
  type: apiKey
- description: Client certificate credential managed via the Certificate resource, supporting mutual-TLS authentication between partner integrations and the Mobile Center orchestration API.
  name: Certificate
  sources:
  - docs
  type: mutualTLS
slug: highway9-authentication
source_filename: highway9-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.highway9.com/mobile-center-streaming-apis/\ndocs: https://www.highway9.com/mobile-center-streaming-apis/\nsummary:\n  types: [apiKey, mutualTLS]\n  api_key_in: [header]\n  note: >-\n    The Mobile Center Streaming APIs expose apiToken and Certificate as managed\n    security resources. Access is issued and administered through the partner\n    portal for signed partners; the full securityScheme definitions live in the\n    partner-gated OpenAPI reference and are not published publicly.\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  description: >-\n    API token credential managed via the apiToken resource. Tokens are issued\n    to signed partners through the Mobile Center partner portal and presented on\n    API requests to the orchestration endpoint.\n  sources: [docs]\n- name: Certificate\n  type: mutualTLS\n  description: >-\n    Client certificate credential managed via the Certificate resource,\n\
  \    supporting mutual-TLS authentication between partner integrations and the\n    Mobile Center orchestration API.\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highway9/refs/heads/main/authentication/highway9-authentication.yml
summary_line: apiKey/mutualTLS · 2 schemes
tags:
- Company
- Networking
- 5G
- Private Mobile Networks
- Wireless
- Edge Computing
- Cloud
- IoT
- Telecommunications
- Enterprise Connectivity
---
