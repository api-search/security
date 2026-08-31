---
api_key_in: []
api_specs:
- filename: conversica-conversica-integrations-api-api-openapi.yml
  format: yaml
  label: Conversica Conversica Integrations API
  slug: conversica-conversica-integrations-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conversica/refs/heads/main/openapi/conversica-conversica-integrations-api-api-openapi.yml
- filename: conversica-leads-api-openapi.yml
  format: yaml
  label: Conversica Leads API
  slug: conversica-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conversica/refs/heads/main/openapi/conversica-leads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Conversica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conversica secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Conversica
provider_slug: conversica
scheme_count: 1
schemes:
- applies_to:
  - direction: customer-to-conversica
    endpoint: https://integrations-api.conversica.com/json/
    operation: postLead
  - direction: conversica-to-customer
    endpoint: customer-hosted
    operation: receiveMessage
  - direction: conversica-to-customer
    endpoint: customer-hosted
    operation: receiveLeadUpdate
  - direction: conversica-to-customer
    endpoint: customer-hosted
    operation: receiveChatLead
  description: 'HTTPS basic access authentication. Conversica issues a username and password for

    the Conversica endpoint; the customer issues a single username/password pair that

    Conversica uses for both customer endpoints. API usernames have a five-character

    minimum. Credentials are obtained from a Conversica technical account manager.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/conversica-integrations-api-openapi.yml
  type: http
slug: conversica-authentication
source_filename: conversica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/conversica-integrations-api-openapi.yml\ndocs: https://help.conversica.com/hc/en-us/articles/360048601712-Conversica-API-Integration-Manual\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  api_key_in: []\n  oauth2_flows: []\n  bidirectional: true\n  note: >-\n    Conversica's API is authenticated in both directions with HTTP Basic over HTTPS.\n    Conversica issues one credential pair for its own endpoint; the customer issues a\n    single credential pair that Conversica uses for every customer-hosted endpoint.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTPS basic access authentication. Conversica issues a username and password for\n    the Conversica endpoint; the customer issues a single username/password pair that\n    Conversica uses for both customer endpoints. API usernames have a five-character\n    minimum. Credentials are obtained from a Conversica technical\
  \ account manager.\n  sources:\n  - openapi/conversica-integrations-api-openapi.yml\n  applies_to:\n  - operation: postLead\n    direction: customer-to-conversica\n    endpoint: https://integrations-api.conversica.com/json/\n  - operation: receiveMessage\n    direction: conversica-to-customer\n    endpoint: customer-hosted\n  - operation: receiveLeadUpdate\n    direction: conversica-to-customer\n    endpoint: customer-hosted\n  - operation: receiveChatLead\n    direction: conversica-to-customer\n    endpoint: customer-hosted\ncredential_lifecycle:\n  self_serve: false\n  issuance: >-\n    Requested from the customer's Conversica technical account manager when the customer is\n    ready for development. Applications must additionally be tested and approved by\n    Conversica before they may be enabled.\n  constraints:\n  - Five character minimum for API usernames.\n  - Both customer endpoints must share one username/password pair.\n  rotation_policy_published: false\n  expiry: none - credentials\
  \ are long-lived shared secrets\n  scopes: none - Basic auth carries no scope or permission model\noauth2:\n  supported: true\n  direction: conversica-to-customer\n  description: >-\n    Conversica documents OAuth 2.0 as an alternative for authenticating Conversica's\n    outbound calls into a customer's own API, so the customer does not have to share direct\n    user credentials. Setup is arranged through a technical account manager or a support\n    case to support@conversica.com.\n  authorization_url: null\n  token_url: null\n  grant_types_published: false\n  scopes_published: false\n  note: >-\n    Because no endpoints, grant types or scopes are published, no scopes artifact is\n    derivable and derive-oauth-scopes.py correctly returns zero.\n  source: https://help.conversica.com/hc/en-us/articles/5357137175835-OAuth-2-0-Authentication-with-Conversica\nobserved:\n  probed: '2026-08-13'\n  endpoint: https://integrations-api.conversica.com/json/\n  challenge_header: 'www-authenticate:\
  \ Basic realm=\"Conversica\"'\n  unauthenticated_status: 401\n  unauthenticated_body: '{\"message\":\"Invalid username or password. Additional failed attempts may result in your account being locked or your IP address being banned.\"}'\n  lockout_policy:\n    published: false\n    observed_warning: true\n    note: >-\n      The live 401 warns that repeated failures may lock the account or ban the source IP.\n      No threshold, lockout duration or unban path is published anywhere in the help centre,\n      so a client cannot implement a safe retry policy from the documented surface. Treat 401\n      as terminal, not retryable.\n  detail: errors/conversica-problem-types.yml\nnot_supported:\n  api_keys: true\n  bearer_tokens: true\n  openid_connect: true\n  mutual_tls: true\n  webhook_signing: true\n  note: >-\n    Each of the above was searched for in the published documentation and probed where\n    applicable (/.well-known/openid-configuration returns 404 on every Conversica host).\n\
  \    There is no webhook signature or HMAC contract, so Basic auth is the whole of the\n    authentication story on the inbound callbacks.\nx-evidence:\n  fetched: '2026-08-01'\n  urls:\n  - url: https://help.conversica.com/hc/en-us/articles/360048601712-Conversica-API-Integration-Manual\n    http_status: 200\n  - url: https://help.conversica.com/hc/en-us/articles/5357137175835-OAuth-2-0-Authentication-with-Conversica\n    http_status: 200\n  - url: https://help.conversica.com/hc/en-us/articles/38828763556635-Implementing-a-Conversica-API-Lead-Creation-Webhook-for-Website-Chat\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conversica/refs/heads/main/authentication/conversica-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Conversational AI
- AI Agents
- Sales
- Marketing
- Lead Management
- CRM
- Marketing Automation
- Customer Engagement
- Messaging
- SMS
- Email
- Chat
- Automotive
- Higher Education
- Webhook
---
