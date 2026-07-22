---
api_key_in: []
auth_types: []
description: Authentication profile for Teads developer APIs. Both public REST surfaces use static API-key style credentials issued out-of-band (via Teads Ad Manager or a Teads account representative); no OAuth 2.0 or OpenID Connect flow is documented.
kind: authentication
layout: security
method: searched
name: Teads Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teads declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Teads
provider_slug: teads
scheme_count: 0
schemes: []
slug: teads-authentication
source_filename: teads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.teads.com/\ndescription: >-\n  Authentication profile for Teads developer APIs. Both public REST surfaces use\n  static API-key style credentials issued out-of-band (via Teads Ad Manager or a\n  Teads account representative); no OAuth 2.0 or OpenID Connect flow is documented.\napis:\n- name: Teads Conversions API\n  schemes:\n  - type: apiKey\n    name: Conversion API Token\n    in: token\n    location: request payload / connector config\n    provisioning: >-\n      Generated in Teads Ad Manager under Settings > Conversion API Tokens >\n      Generate Conversion API Token. Shown once; must be stored securely.\n    docs: https://docs.tealium.com/server-side-connectors/teads-conversions-connector/\n- name: Teads In-Chat API\n  schemes:\n  - type: apiKey\n    name: key\n    in: query\n    provisioning: >-\n      Unique Partner API Key obtained from a Teads account representative and\n      passed as the `key`\
  \ request parameter. Requests also require User-Agent and\n      X-Forwarded-For headers carrying the end-user agent and IP.\n    docs: https://developers.teads.com/docs/Chatbot-AI-SDK/Getting-Started/integration-guide/\nnotes: >-\n  No OpenAPI document is published by Teads, so this profile is derived from the\n  developer portal and partner integration documentation rather than a machine\n  spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teads/refs/heads/main/authentication/teads-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Advertising
- AdTech
- Advertising Technology
- Video Advertising
- Conversions API
- Contextual Advertising
- Mobile SDK
- Conversational AI
---
