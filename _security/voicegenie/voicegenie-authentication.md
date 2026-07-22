---
api_key_in:
- body
api_specs:
- filename: voicegenie-openapi.yml
  format: yaml
  label: VoiceGenie Public REST API
  slug: voicegenie-public-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voicegenie/refs/heads/main/openapi/voicegenie-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Voicegenie Authentication
name_suffix: Authentication
oauth_flows: []
overview: VoiceGenie secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VoiceGenie
provider_slug: voicegenie
scheme_count: 3
schemes:
- description: API token for the pushCallToCampaign endpoint. Generated in the dashboard under Developer APIs -> Generate Token. Sent in the JSON body.
  field: token
  in: body
  name: apiToken
  sources:
  - https://voicegenie.gitbook.io/voicegenie-ai/developer-documentation-1.0
  type: apiKey
- description: Developer API key for the publicRestApiActions endpoints. Copied/regenerated in the dashboard under System -> APIs. Sent in the JSON body. Keep private.
  field: apiKey
  in: body
  name: apiKey
  sources:
  - https://voicegenie.gitbook.io/voicegenie-ai/integrations/public-api-integration
  type: apiKey
- description: Workspace identifier required alongside the token/apiKey. Constant for the account even when the token is regenerated.
  field: workspaceId
  in: body
  name: workspaceId
  sources:
  - https://voicegenie.gitbook.io/voicegenie-ai/integrations/public-api-integration
  type: apiKey
slug: voicegenie-authentication
source_filename: voicegenie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://voicegenie.gitbook.io/voicegenie-ai/developer-documentation-1.0\ndocs: https://voicegenie.gitbook.io/voicegenie-ai/integrations/public-api-integration\nsummary:\n  types: [apiKey]\n  api_key_in: [body]\n  oauth2_flows: []\n  note: >-\n    VoiceGenie authenticates by including an API token and a workspaceId inside the JSON request\n    payload (not an HTTP header). This is a non-standard, body-carried API-key scheme, so it is not\n    expressed as an OpenAPI securityScheme; the credential fields are documented as required request\n    properties instead.\nschemes:\n- name: apiToken\n  type: apiKey\n  in: body\n  field: token\n  description: >-\n    API token for the pushCallToCampaign endpoint. Generated in the dashboard under\n    Developer APIs -> Generate Token. Sent in the JSON body.\n  sources: [https://voicegenie.gitbook.io/voicegenie-ai/developer-documentation-1.0]\n- name: apiKey\n  type: apiKey\n  in: body\n\
  \  field: apiKey\n  description: >-\n    Developer API key for the publicRestApiActions endpoints. Copied/regenerated in the dashboard\n    under System -> APIs. Sent in the JSON body. Keep private.\n  sources: [https://voicegenie.gitbook.io/voicegenie-ai/integrations/public-api-integration]\n- name: workspaceId\n  type: apiKey\n  in: body\n  field: workspaceId\n  description: >-\n    Workspace identifier required alongside the token/apiKey. Constant for the account even when the\n    token is regenerated.\n  sources: [https://voicegenie.gitbook.io/voicegenie-ai/integrations/public-api-integration]\ntoken_management:\n  generate: Dashboard -> Developer APIs -> Generate Token (or System -> APIs -> Regenerate Token)\n  rotation: Regenerating the token does not change the workspaceId.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voicegenie/refs/heads/main/authentication/voicegenie-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Voice AI
- Conversational AI
- Sales Automation
- Voice Agents
- Telephony
- Call Center
- Customer Support
- Lead Generation
- Webhooks
---
