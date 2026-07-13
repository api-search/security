---
api_key_in:
- header
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fabric Origin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fabric Origin secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fabric Origin
provider_slug: fabric-origin
scheme_count: 2
schemes:
- in: header
  name: SubscriptionKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/fabric-origin-openapi.yml
  type: apiKey
- in: query
  name: SubscriptionKeyQuery
  parameter: subscription-key
  sources:
  - openapi/fabric-origin-openapi.yml
  type: apiKey
slug: fabric-origin-authentication
source_filename: fabric-origin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fabric-origin-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: SubscriptionKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/fabric-origin-openapi.yml\n- name: SubscriptionKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/fabric-origin-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/authentication/fabric-origin-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Entertainment
- Movies
- Television
- Games
- Trailers
- Metadata
---
