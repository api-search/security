---
api_key_in: []
api_specs:
- filename: sendpulse-bulk-email-openapi.yml
  format: yaml
  label: SendPulse Bulk Email API
  slug: sendpulse-bulk-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-bulk-email-openapi.yml
- filename: sendpulse-smtp-openapi.yml
  format: yaml
  label: SendPulse SMTP API
  slug: sendpulse-smtp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-smtp-openapi.yml
- filename: sendpulse-sms-openapi.yml
  format: yaml
  label: SendPulse SMS API
  slug: sendpulse-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-sms-openapi.yml
- filename: sendpulse-crm-openapi.yml
  format: yaml
  label: SendPulse CRM Public API
  slug: sendpulse-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-crm-openapi.yml
- filename: sendpulse-a360-openapi.yml
  format: yaml
  label: SendPulse Automation 360 API
  slug: sendpulse-a360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-a360-openapi.yml
- filename: sendpulse-chatbots-openapi.yml
  format: yaml
  label: SendPulse Chatbots Service API
  slug: sendpulse-chatbots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-chatbots-openapi.yml
- filename: sendpulse-whatsapp-openapi.yml
  format: yaml
  label: SendPulse WhatsApp Chatbot API
  slug: sendpulse-whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-whatsapp-openapi.yml
- filename: sendpulse-telegram-openapi.yml
  format: yaml
  label: SendPulse Telegram Chatbot API
  slug: sendpulse-telegram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-telegram-openapi.yml
- filename: sendpulse-facebook-openapi.yml
  format: yaml
  label: SendPulse Facebook Messenger Chatbot API
  slug: sendpulse-facebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-facebook-openapi.yml
- filename: sendpulse-instagram-openapi.yml
  format: yaml
  label: SendPulse Instagram Chatbot API
  slug: sendpulse-instagram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-instagram-openapi.yml
- filename: sendpulse-viber-chatbot-openapi.yml
  format: yaml
  label: SendPulse Viber Chatbot API
  slug: sendpulse-viber-chatbot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-viber-chatbot-openapi.yml
- filename: sendpulse-tiktok-openapi.yml
  format: yaml
  label: SendPulse TikTok Chatbot API
  slug: sendpulse-tiktok-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-tiktok-openapi.yml
- filename: sendpulse-live-chat-openapi.yml
  format: yaml
  label: SendPulse LiveChat API
  slug: sendpulse-live-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-live-chat-openapi.yml
- filename: sendpulse-web-push-openapi.yml
  format: yaml
  label: SendPulse Web Push API
  slug: sendpulse-web-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-web-push-openapi.yml
- filename: sendpulse-viber-openapi.yml
  format: yaml
  label: SendPulse Viber API
  slug: sendpulse-viber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-viber-openapi.yml
- filename: sendpulse-verifier-openapi.yml
  format: yaml
  label: SendPulse Verifier API
  slug: sendpulse-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-verifier-openapi.yml
- filename: sendpulse-edu-openapi.yml
  format: yaml
  label: SendPulse Education API
  slug: sendpulse-edu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-edu-openapi.yml
- filename: sendpulse-popups-openapi.yml
  format: yaml
  label: SendPulse Pop-up API
  slug: sendpulse-popups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-popups-openapi.yml
- filename: sendpulse-file-manager-openapi.yml
  format: yaml
  label: SendPulse File Manager API
  slug: sendpulse-file-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-file-manager-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sendpulse Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SendPulse secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SendPulse
provider_slug: sendpulse
scheme_count: 2
schemes:
- bearerFormat: API Key
  description: Static API Key authentication.  A long-lived token generated manually in the SendPulse account settings.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/sendpulse-a360-openapi.yml
  - openapi/sendpulse-bulk-email-openapi.yml
  - openapi/sendpulse-chatbots-openapi.yml
  - openapi/sendpulse-crm-openapi.yml
  - openapi/sendpulse-edu-openapi.yml
  - openapi/sendpulse-facebook-openapi.yml
  - openapi/sendpulse-file-manager-openapi.yml
  - openapi/sendpulse-instagram-openapi.yml
  - openapi/sendpulse-live-chat-openapi.yml
  - openapi/sendpulse-popups-openapi.yml
  - openapi/sendpulse-sms-openapi.yml
  - openapi/sendpulse-smtp-openapi.yml
  - openapi/sendpulse-telegram-openapi.yml
  - openapi/sendpulse-tiktok-openapi.yml
  - openapi/sendpulse-verifier-openapi.yml
  - openapi/sendpulse-viber-chatbot-openapi.yml
  - openapi/sendpulse-viber-openapi.yml
  - openapi/sendpulse-web-push-openapi.yml
  - openapi/sendpulse-whatsapp-openapi.yml
  type: http
- description: OAuth 2.0 Client Credentials flow for temporary access tokens.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.sendpulse.com/oauth/access_token
  name: oauth2
  sources:
  - openapi/sendpulse-a360-openapi.yml
  - openapi/sendpulse-bulk-email-openapi.yml
  - openapi/sendpulse-chatbots-openapi.yml
  - openapi/sendpulse-crm-openapi.yml
  - openapi/sendpulse-edu-openapi.yml
  - openapi/sendpulse-facebook-openapi.yml
  - openapi/sendpulse-file-manager-openapi.yml
  - openapi/sendpulse-instagram-openapi.yml
  - openapi/sendpulse-live-chat-openapi.yml
  - openapi/sendpulse-popups-openapi.yml
  - openapi/sendpulse-sms-openapi.yml
  - openapi/sendpulse-smtp-openapi.yml
  - openapi/sendpulse-telegram-openapi.yml
  - openapi/sendpulse-tiktok-openapi.yml
  - openapi/sendpulse-verifier-openapi.yml
  - openapi/sendpulse-viber-chatbot-openapi.yml
  - openapi/sendpulse-viber-openapi.yml
  - openapi/sendpulse-web-push-openapi.yml
  - openapi/sendpulse-whatsapp-openapi.yml
  type: oauth2
slug: sendpulse-authentication
source_filename: sendpulse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://sendpulse.com/integrations/api + https://api.sendpulse.com/service-directory.json + openapi/*.yml\n  (securitySchemes across all 19 published specs)\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  header: 'Authorization: Bearer <token_or_key>'\n  token_endpoint: https://api.sendpulse.com/oauth/access_token\n  token_ttl_seconds: 3600\n  api_key_max_per_account: 5\n  credentials_page: https://login.sendpulse.com/settings/#api\n  scopes: none on the REST API; the MCP server advertises a single \"rest\" scope — see scopes/sendpulse-scopes.yml\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: Static API Key authentication.  A long-lived token generated manually in the SendPulse account settings.\n  sources:\n  - openapi/sendpulse-a360-openapi.yml\n  - openapi/sendpulse-bulk-email-openapi.yml\n  - openapi/sendpulse-chatbots-openapi.yml\n\
  \  - openapi/sendpulse-crm-openapi.yml\n  - openapi/sendpulse-edu-openapi.yml\n  - openapi/sendpulse-facebook-openapi.yml\n  - openapi/sendpulse-file-manager-openapi.yml\n  - openapi/sendpulse-instagram-openapi.yml\n  - openapi/sendpulse-live-chat-openapi.yml\n  - openapi/sendpulse-popups-openapi.yml\n  - openapi/sendpulse-sms-openapi.yml\n  - openapi/sendpulse-smtp-openapi.yml\n  - openapi/sendpulse-telegram-openapi.yml\n  - openapi/sendpulse-tiktok-openapi.yml\n  - openapi/sendpulse-verifier-openapi.yml\n  - openapi/sendpulse-viber-chatbot-openapi.yml\n  - openapi/sendpulse-viber-openapi.yml\n  - openapi/sendpulse-web-push-openapi.yml\n  - openapi/sendpulse-whatsapp-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.sendpulse.com/oauth/access_token\n    scopes: 0\n  description: OAuth 2.0 Client Credentials flow for temporary access tokens.\n  sources:\n  - openapi/sendpulse-a360-openapi.yml\n  - openapi/sendpulse-bulk-email-openapi.yml\n\
  \  - openapi/sendpulse-chatbots-openapi.yml\n  - openapi/sendpulse-crm-openapi.yml\n  - openapi/sendpulse-edu-openapi.yml\n  - openapi/sendpulse-facebook-openapi.yml\n  - openapi/sendpulse-file-manager-openapi.yml\n  - openapi/sendpulse-instagram-openapi.yml\n  - openapi/sendpulse-live-chat-openapi.yml\n  - openapi/sendpulse-popups-openapi.yml\n  - openapi/sendpulse-sms-openapi.yml\n  - openapi/sendpulse-smtp-openapi.yml\n  - openapi/sendpulse-telegram-openapi.yml\n  - openapi/sendpulse-tiktok-openapi.yml\n  - openapi/sendpulse-verifier-openapi.yml\n  - openapi/sendpulse-viber-chatbot-openapi.yml\n  - openapi/sendpulse-viber-openapi.yml\n  - openapi/sendpulse-web-push-openapi.yml\n  - openapi/sendpulse-whatsapp-openapi.yml\ndocs: https://sendpulse.com/integrations/api\nnotes:\n- 'Both methods travel in the same Authorization: Bearer header, so a server cannot tell a short-lived OAuth token\n  from a permanent API key by the request alone.'\n- A static API key never expires and carries\
  \ full account permissions; up to 5 per account.\n- The token endpoint POST /oauth/access_token is documented but is NOT declared as an operation in any of the 19\n  published OpenAPI specs — a client generated purely from the specs cannot authenticate.\n- One spec (chatbots, crm, edu, facebook, file-manager, instagram, live-chat, popups, telegram, tiktok, viber-chatbot,\n  whatsapp) misspells the scheme key as \"outh2\" rather than \"oauth2\"; it is a naming typo in the published contract,\n  not a different mechanism.\n- The MCP server at mcp.sendpulse.com uses a separate authorization_code + PKCE flow with dynamic client registration,\n  or X-SP-ID / X-SP-SECRET headers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/authentication/sendpulse-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Marketing
- Marketing Automation
- Email
- Transactional Email
- SMS
- Web Push
- Chatbots
- CRM
- Multi-Channel
- Messaging
- Online Courses
- Popups
- Email Verification
- MCP
- Agent Ready
---
