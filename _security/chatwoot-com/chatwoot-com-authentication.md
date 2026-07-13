---
api_key_in:
- header
api_specs:
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Agents API
  slug: chatwoot-application-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Teams API
  slug: chatwoot-application-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Inboxes API
  slug: chatwoot-application-inboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Contacts API
  slug: chatwoot-application-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Conversations API
  slug: chatwoot-application-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Messages API
  slug: chatwoot-application-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Labels API
  slug: chatwoot-application-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Custom Attributes API
  slug: chatwoot-application-custom-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Canned Responses API
  slug: chatwoot-application-canned-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Automation Rules API
  slug: chatwoot-application-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Application Reports API
  slug: chatwoot-application-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Client Contacts API
  slug: chatwoot-client-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Client Conversations API
  slug: chatwoot-client-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Client Messages API
  slug: chatwoot-client-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Platform Users API
  slug: chatwoot-platform-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Platform Accounts API
  slug: chatwoot-platform-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
- filename: chatwoot-com-openapi.yml
  format: yaml
  label: Chatwoot Platform Agent Bots API
  slug: chatwoot-platform-agent-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwoot-com/refs/heads/main/openapi/chatwoot-com-openapi.yml
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
