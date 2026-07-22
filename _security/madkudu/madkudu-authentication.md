---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Madkudu Authentication
name_suffix: Authentication
oauth_flows: []
overview: MadKudu secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MadKudu
provider_slug: madkudu
scheme_count: 2
schemes:
- applies_to: MadKudu API (MadAPI)
  description: The current MadKudu API (MadAPI) authenticates with a raw API key sent in the X-API-Key request header. Base URL https://madapi.madkudu.com (staging https://madapi.wisekudu.com). Applies to all MadAPI endpoints.
  in: header
  name: MadAPIKey
  parameter_name: X-API-Key
  type: apiKey
- applies_to: MadKudu Legacy Scoring API
  description: 'The legacy Scoring API uses HTTP Basic authentication with the API key as the username and an empty password, i.e. Authorization: Basic base64(YOUR_API_KEY:). Base URL https://api.madkudu.com.'
  name: LegacyBasicAuth
  scheme: basic
  type: http
slug: madkudu-authentication
source_filename: madkudu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developers.madkudu.com/getting-started\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  http_schemes: [basic]\n  oauth2_flows: []\nschemes:\n- name: MadAPIKey\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  description: >-\n    The current MadKudu API (MadAPI) authenticates with a raw API key sent in the\n    X-API-Key request header. Base URL https://madapi.madkudu.com (staging\n    https://madapi.wisekudu.com). Applies to all MadAPI endpoints.\n  applies_to: MadKudu API (MadAPI)\n- name: LegacyBasicAuth\n  type: http\n  scheme: basic\n  description: >-\n    The legacy Scoring API uses HTTP Basic authentication with the API key as the\n    username and an empty password, i.e. Authorization: Basic base64(YOUR_API_KEY:).\n    Base URL https://api.madkudu.com.\n  applies_to: MadKudu Legacy Scoring API\nnotes: >-\n  API keys are issued from the MadKudu account settings. The MCP server embeds\
  \ the\n  same API key as a path segment in the server URL (see mcp/madkudu-mcp.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madkudu/refs/heads/main/authentication/madkudu-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Applicative Saas
- Sales Intelligence
- Lead Scoring
- Predictive Analytics
- Account Intelligence
- Data Enrichment
- MCP
---
