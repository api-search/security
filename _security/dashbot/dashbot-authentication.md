---
api_key_in:
- header
- query
api_specs:
- filename: dashbot-export-openapi.json
  format: json
  label: Dashbot / Dimension Labs Export API
  slug: dashbot-dimension-labs-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dashbot/refs/heads/main/openapi/dashbot-export-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dashbot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dashbot secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dashbot
provider_slug: dashbot
scheme_count: 2
schemes:
- description: API key passed in the Authorization header on the Export API (GET https://api.dimensionlabs.io/export). Keys are generated per integration/source in the Dimension Labs app (Integrations > Add Source > Show Integration Instructions).
  in: header
  name: AuthorizationHeader
  parameter: Authorization
  sources:
  - openapi/dashbot-export-openapi.json
  type: apiKey
- description: API key supplied with realtime ingest calls to the Universal tracker endpoint (https://tracker.dimensionlabs.io/track?platform=universal). Each integration source has its own key generated in the Dimension Labs app.
  in: query
  name: TrackerApiKey
  parameter: apiKey
  sources:
  - https://docs.dimensionlabs.io/reference/rest-api
  type: apiKey
slug: dashbot-authentication
source_filename: dashbot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.dimensionlabs.io/reference/generating-dashbot-api-key + openapi/dashbot-export-openapi.json\ndocs: https://docs.dimensionlabs.io/reference/generating-dashbot-api-key\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\nschemes:\n- name: AuthorizationHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    API key passed in the Authorization header on the Export API\n    (GET https://api.dimensionlabs.io/export). Keys are generated per\n    integration/source in the Dimension Labs app (Integrations > Add Source >\n    Show Integration Instructions).\n  sources: [openapi/dashbot-export-openapi.json]\n- name: TrackerApiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: >-\n    API key supplied with realtime ingest calls to the Universal tracker\n    endpoint (https://tracker.dimensionlabs.io/track?platform=universal). Each\n    integration\
  \ source has its own key generated in the Dimension Labs app.\n  sources: [https://docs.dimensionlabs.io/reference/rest-api]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dashbot/refs/heads/main/authentication/dashbot-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Ai Ml
- Conversational Analytics
- Chatbots
- Voice Assistants
- Customer Experience
- Data Enrichment
- Analytics
- Contact Center
---
