---
api_key_in:
- header
api_specs:
- filename: chatwoot-com-agents-api-openapi.yml
  format: yaml
  label: Chatwoot Agents API
  slug: chatwoot-com-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-agents-api-openapi.yml
- filename: chatwoot-com-automation-rules-api-openapi.yml
  format: yaml
  label: Chatwoot Automation Rules API
  slug: chatwoot-com-automation-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-automation-rules-api-openapi.yml
- filename: chatwoot-com-canned-responses-api-openapi.yml
  format: yaml
  label: Chatwoot Canned Responses API
  slug: chatwoot-com-canned-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-canned-responses-api-openapi.yml
- filename: chatwoot-com-client-contacts-api-openapi.yml
  format: yaml
  label: Chatwoot Client Contacts API
  slug: chatwoot-com-client-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-client-contacts-api-openapi.yml
- filename: chatwoot-com-client-conversations-api-openapi.yml
  format: yaml
  label: Chatwoot Client Conversations API
  slug: chatwoot-com-client-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-client-conversations-api-openapi.yml
- filename: chatwoot-com-client-messages-api-openapi.yml
  format: yaml
  label: Chatwoot Client Messages API
  slug: chatwoot-com-client-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-client-messages-api-openapi.yml
- filename: chatwoot-com-contacts-api-openapi.yml
  format: yaml
  label: Chatwoot Contacts API
  slug: chatwoot-com-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-contacts-api-openapi.yml
- filename: chatwoot-com-conversations-api-openapi.yml
  format: yaml
  label: Chatwoot Conversations API
  slug: chatwoot-com-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-conversations-api-openapi.yml
- filename: chatwoot-com-custom-attributes-api-openapi.yml
  format: yaml
  label: Chatwoot Custom Attributes API
  slug: chatwoot-com-custom-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-custom-attributes-api-openapi.yml
- filename: chatwoot-com-inboxes-api-openapi.yml
  format: yaml
  label: Chatwoot Inboxes API
  slug: chatwoot-com-inboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-inboxes-api-openapi.yml
- filename: chatwoot-com-labels-api-openapi.yml
  format: yaml
  label: Chatwoot Labels API
  slug: chatwoot-com-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-labels-api-openapi.yml
- filename: chatwoot-com-messages-api-openapi.yml
  format: yaml
  label: Chatwoot Messages API
  slug: chatwoot-com-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-messages-api-openapi.yml
- filename: chatwoot-com-platform-accounts-api-openapi.yml
  format: yaml
  label: Chatwoot Platform Accounts API
  slug: chatwoot-com-platform-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-platform-accounts-api-openapi.yml
- filename: chatwoot-com-platform-agent-bots-api-openapi.yml
  format: yaml
  label: Chatwoot Platform Agent Bots API
  slug: chatwoot-com-platform-agent-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-platform-agent-bots-api-openapi.yml
- filename: chatwoot-com-platform-users-api-openapi.yml
  format: yaml
  label: Chatwoot Platform Users API
  slug: chatwoot-com-platform-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-platform-users-api-openapi.yml
- filename: chatwoot-com-reports-api-openapi.yml
  format: yaml
  label: Chatwoot Reports API
  slug: chatwoot-com-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-reports-api-openapi.yml
- filename: chatwoot-com-teams-api-openapi.yml
  format: yaml
  label: Chatwoot Teams API
  slug: chatwoot-com-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-teams-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Chatwoot Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chatwoot secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chatwoot
provider_slug: chatwoot-com
scheme_count: 1
schemes:
- description: Application and Client access token passed in the `api_access_token` HTTP header. For the Application API this is an agent/user access token; Client API requests are additionally scoped by inbox and contact identifiers.
  in: header
  name: userApiKey
  parameter: api_access_token
  sources:
  - openapi/chatwoot-com-openapi.yml
  type: apiKey
slug: chatwoot-com-authentication
source_filename: chatwoot-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chatwoot-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: userApiKey\n  type: apiKey\n  in: header\n  parameter: api_access_token\n  description: Application and Client access token passed in the `api_access_token` HTTP header.\n    For the Application API this is an agent/user access token; Client API requests are additionally\n    scoped by inbox and contact identifiers.\n  sources:\n  - openapi/chatwoot-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/authentication/chatwoot-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Customer Support
- Customer Engagement
- Shared Inbox
- Live Chat
- Open Source
- Omnichannel
- Help Desk
---
