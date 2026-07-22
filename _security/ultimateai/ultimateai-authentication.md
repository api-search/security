---
api_key_in:
- header
auth_types:
- http-basic
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ultimateai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ultimate.ai secures its APIs with http-basic and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ultimate.ai
provider_slug: ultimateai
scheme_count: 4
schemes:
- description: 'Legacy Chat Automation endpoint (POST /api/v2/automation on chat.ultimate.ai) used Basic Access Authentication - a Base64 encoding of email:password sent as "Authorization: Basic {basicAuthToken}".'
  name: basicAuth (legacy Ultimate.ai Public API)
  scheme: basic
  sources:
  - https://github.com/ultimateai/public-api/blob/main/source/includes/_automation.md
  type: http
- description: Legacy Intent Recognition (POST /api/intents) and Delete User Data (POST /api/gdpr/delete-user-data) endpoints took a bot access token in an "authorization" header. Tokens were found in the dashboard under bot settings > Tokens.
  in: header
  name: accessToken (legacy Ultimate.ai Public API)
  parameter: authorization
  sources:
  - https://github.com/ultimateai/public-api/blob/main/source/includes/_intents.md
  - https://github.com/ultimateai/public-api/blob/main/source/includes/_gdpr.md
  type: apiKey
- description: Successor AI Agents Chat/Ticket/Widget Escalation APIs authenticate with a Custom CRM API key in the Authorization header, generated from the Custom CRM integration page (docs still reference the Ultimate.ai dashboard). A botid header identifies the bot.
  in: header
  name: customCrmApiKey (Zendesk AI Agents API)
  parameter: Authorization
  sources:
  - https://developer.zendesk.com/api-reference/ai-agents/authentication/
  - https://developer.zendesk.com/api-reference/ai-agents/chat/chat/
  type: apiKey
- description: Fallback when no custom CRM integration is configured - an organization API key (Organization management > API Key > Generate) sent with an organizationid HTTP header.
  in: header
  name: organizationApiKey (Zendesk AI Agents API)
  parameter: Authorization
  sources:
  - https://developer.zendesk.com/api-reference/ai-agents/authentication/
  type: apiKey
slug: ultimateai-authentication
source_filename: ultimateai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/ultimateai/public-api\ndocs: https://developer.zendesk.com/api-reference/ai-agents/authentication/\nnotes: >-\n  Ultimate.ai was acquired by Zendesk and its product now ships as Zendesk AI agents\n  (Advanced add-on). Two auth surfaces are documented: the legacy Ultimate.ai Public API\n  (chat.ultimate.ai, Slate docs in github.com/ultimateai/public-api; host now returns 404\n  on probed endpoints) and the successor Zendesk AI Agents API on\n  {subdomain}.zendesk.com/ai-agents/api.\nsummary:\n  types: [http-basic, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: basicAuth (legacy Ultimate.ai Public API)\n  type: http\n  scheme: basic\n  description: >-\n    Legacy Chat Automation endpoint (POST /api/v2/automation on chat.ultimate.ai) used\n    Basic Access Authentication - a Base64 encoding of email:password sent as\n    \"Authorization: Basic {basicAuthToken}\".\n  sources:\n  - https://github.com/ultimateai/public-api/blob/main/source/includes/_automation.md\n\
  - name: accessToken (legacy Ultimate.ai Public API)\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: >-\n    Legacy Intent Recognition (POST /api/intents) and Delete User Data\n    (POST /api/gdpr/delete-user-data) endpoints took a bot access token in an\n    \"authorization\" header. Tokens were found in the dashboard under bot settings > Tokens.\n  sources:\n  - https://github.com/ultimateai/public-api/blob/main/source/includes/_intents.md\n  - https://github.com/ultimateai/public-api/blob/main/source/includes/_gdpr.md\n- name: customCrmApiKey (Zendesk AI Agents API)\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Successor AI Agents Chat/Ticket/Widget Escalation APIs authenticate with a Custom CRM\n    API key in the Authorization header, generated from the Custom CRM integration page\n    (docs still reference the Ultimate.ai dashboard). A botid header identifies the bot.\n  sources:\n  - https://developer.zendesk.com/api-reference/ai-agents/authentication/\n\
  \  - https://developer.zendesk.com/api-reference/ai-agents/chat/chat/\n- name: organizationApiKey (Zendesk AI Agents API)\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Fallback when no custom CRM integration is configured - an organization API key\n    (Organization management > API Key > Generate) sent with an organizationid HTTP header.\n  sources:\n  - https://developer.zendesk.com/api-reference/ai-agents/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ultimateai/refs/heads/main/authentication/ultimateai-authentication.yml
summary_line: http-basic/apiKey · 4 schemes
tags:
- Company
- Ai Enterprise Software
- Customer Support
- Conversational AI
- Chatbots
- AI Agents
- Automation
- Acquired
---
