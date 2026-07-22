---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Media Radar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Media Radar secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Media Radar
provider_slug: media-radar
scheme_count: 1
schemes:
- description: Per-client MediaRadar API Key issued through the Client API Portal, presented as an Azure API Management subscription key header on each request.
  in: header
  name: apiKey
  sources:
  - https://api-portal.mediaradar.com/
  type: apiKey
slug: media-radar-authentication
source_filename: media-radar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api-portal.mediaradar.com/\ndocs: https://api-portal.mediaradar.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nnotes: >-\n  MediaRadar exposes its data through the MediaRadar Client API Portal, a private\n  Azure API Management developer portal (api-portal.mediaradar.com). Access is\n  gated behind a client sign-in / OAuth sign-up; API definitions, endpoints, and\n  request/response schemas are not published publicly. Documentation confirms\n  authentication is performed with a per-client API Key. As an Azure API\n  Management surface the key is supplied as a subscription-key request header\n  (Ocp-Apim-Subscription-Key by APIM default). No OpenAPI spec was publicly\n  retrievable to mechanically derive securitySchemes, so this profile is sourced\n  from the provider's public portal and integration guidance rather than a spec.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n\
  \  description: >-\n    Per-client MediaRadar API Key issued through the Client API Portal, presented\n    as an Azure API Management subscription key header on each request.\n  sources:\n  - https://api-portal.mediaradar.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/media-radar/refs/heads/main/authentication/media-radar-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Commerce
- Advertising Intelligence
- Marketing Intelligence
- Competitive Intelligence
- Advertising
- Media
- Data
---
