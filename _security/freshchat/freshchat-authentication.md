---
api_key_in: []
api_specs:
- filename: freshchat-accounts-api-openapi.yml
  format: yaml
  label: Freshchat Accounts API
  slug: freshchat-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-accounts-api-openapi.yml
- filename: freshchat-agents-api-openapi.yml
  format: yaml
  label: Freshchat Agents API
  slug: freshchat-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-agents-api-openapi.yml
- filename: freshchat-businesshours-api-openapi.yml
  format: yaml
  label: Freshchat BusinessHours API
  slug: freshchat-businesshours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-businesshours-api-openapi.yml
- filename: freshchat-channels-api-openapi.yml
  format: yaml
  label: Freshchat Channels API
  slug: freshchat-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-channels-api-openapi.yml
- filename: freshchat-conversations-api-openapi.yml
  format: yaml
  label: Freshchat Conversations API
  slug: freshchat-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-conversations-api-openapi.yml
- filename: freshchat-csat-api-openapi.yml
  format: yaml
  label: Freshchat CSAT API
  slug: freshchat-csat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-csat-api-openapi.yml
- filename: freshchat-files-api-openapi.yml
  format: yaml
  label: Freshchat Files API
  slug: freshchat-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-files-api-openapi.yml
- filename: freshchat-groups-api-openapi.yml
  format: yaml
  label: Freshchat Groups API
  slug: freshchat-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-groups-api-openapi.yml
- filename: freshchat-messages-api-openapi.yml
  format: yaml
  label: Freshchat Messages API
  slug: freshchat-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-messages-api-openapi.yml
- filename: freshchat-metrics-api-openapi.yml
  format: yaml
  label: Freshchat Metrics API
  slug: freshchat-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-metrics-api-openapi.yml
- filename: freshchat-outboundmessages-api-openapi.yml
  format: yaml
  label: Freshchat OutboundMessages API
  slug: freshchat-outboundmessages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-outboundmessages-api-openapi.yml
- filename: freshchat-roles-api-openapi.yml
  format: yaml
  label: Freshchat Roles API
  slug: freshchat-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-roles-api-openapi.yml
- filename: freshchat-users-api-openapi.yml
  format: yaml
  label: Freshchat Users API
  slug: freshchat-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Freshchat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freshchat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freshchat
provider_slug: freshchat
scheme_count: 1
schemes:
- description: Bearer API token generated in the Freshchat admin console.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/freshchat-openapi.yml
  type: http
slug: freshchat-authentication
source_filename: freshchat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freshchat-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer API token generated in the Freshchat admin console.\n  sources:\n  - openapi/freshchat-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/authentication/freshchat-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Messaging
- Live Chat
- Customer-Support
- Conversational Engagement
- Omnichannel Messaging
- Chatbots
- Freshworks
---
