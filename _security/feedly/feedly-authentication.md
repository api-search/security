---
api_key_in:
- header
api_specs:
- filename: feedly-streams-openapi.yml
  format: yaml
  label: Feedly API
  slug: feedly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feedly/refs/heads/main/openapi/feedly-streams-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Feedly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Feedly secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Feedly
provider_slug: feedly
scheme_count: 2
schemes:
- bearerFormat: token
  description: 'Pass your Feedly API Access Token in the `Authorization` header as a Bearer token, e.g. `Authorization: Bearer <token>`. See [Authorization](https://developers.feedly.com/reference/authorization) for how to generate one.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/feedly-agents-openapi.yml
  - openapi/feedly-enterprise-collections-openapi.yml
  - openapi/feedly-enterprise-users-openapi.yml
  - openapi/feedly-intel-profiles-openapi.yml
  - openapi/feedly-iocs-openapi.yml
  - openapi/feedly-ti-endpoints-openapi.yml
  type: http
- in: header
  name: sec0
  parameter: Authorization
  sources:
  - openapi/feedly-alerts-openapi.yml
  - openapi/feedly-annotations-openapi.yml
  - openapi/feedly-enterprise-openapi.yml
  - openapi/feedly-entities-openapi.yml
  - openapi/feedly-entries-openapi.yml
  - openapi/feedly-memes-openapi.yml
  - openapi/feedly-ml-openapi.yml
  - openapi/feedly-search-openapi.yml
  - openapi/feedly-streams-openapi.yml
  - openapi/feedly-tags-openapi.yml
  - openapi/feedly-trends-openapi.yml
  type: apiKey
slug: feedly-authentication
source_filename: feedly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/feedly-agents-openapi.yml, openapi/feedly-alerts-openapi.yml, openapi/feedly-annotations-openapi.yml,\n  openapi/feedly-enterprise-collections-openapi.yml, openapi/feedly-enterprise-openapi.yml,\n  openapi/feedly-enterprise-users-openapi.yml, openapi/feedly-entities-openapi.yml, openapi/feedly-entries-openapi.yml,\n  openapi/feedly-intel-profiles-openapi.yml, openapi/feedly-iocs-openapi.yml, openapi/feedly-memes-openapi.yml,\n  openapi/feedly-ml-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: 'Pass your Feedly API Access Token in the `Authorization` header as a Bearer\n    token, e.g. `Authorization: Bearer <token>`. See [Authorization](https://developers.feedly.com/reference/authorization)\n    for how to generate one.'\n  sources:\n  - openapi/feedly-agents-openapi.yml\n  - openapi/feedly-enterprise-collections-openapi.yml\n\
  \  - openapi/feedly-enterprise-users-openapi.yml\n  - openapi/feedly-intel-profiles-openapi.yml\n  - openapi/feedly-iocs-openapi.yml\n  - openapi/feedly-ti-endpoints-openapi.yml\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/feedly-alerts-openapi.yml\n  - openapi/feedly-annotations-openapi.yml\n  - openapi/feedly-enterprise-openapi.yml\n  - openapi/feedly-entities-openapi.yml\n  - openapi/feedly-entries-openapi.yml\n  - openapi/feedly-memes-openapi.yml\n  - openapi/feedly-ml-openapi.yml\n  - openapi/feedly-search-openapi.yml\n  - openapi/feedly-streams-openapi.yml\n  - openapi/feedly-tags-openapi.yml\n  - openapi/feedly-trends-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feedly/refs/heads/main/authentication/feedly-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Threat Intelligence
- Cybersecurity
- cyber-threat-intelligence
- Content Aggregation
- RSS
- News
- Vulnerability Management
- Indicators of Compromise
- Malware
- threat-actors
- mitre-attack
- Security Automation
- Artificial Intelligence
- MCP
- agent-native
- Webhook
---
