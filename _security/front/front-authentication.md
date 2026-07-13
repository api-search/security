---
api_key_in: []
api_specs:
- filename: front-core-api-openapi.json
  format: json
  label: Front Conversations API
  slug: front-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Messages API
  slug: front-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Drafts API
  slug: front-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Channels API
  slug: front-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Inboxes API
  slug: front-inboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Contacts API
  slug: front-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Contact Groups API
  slug: front-contact-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Accounts API
  slug: front-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Teammates API
  slug: front-teammates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Teams API
  slug: front-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Comments API
  slug: front-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Tags API
  slug: front-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Topics API
  slug: front-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Rules API
  slug: front-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Signatures API
  slug: front-signatures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Shifts API
  slug: front-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Knowledge Base API
  slug: front-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Analytics API
  slug: front-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Events API
  slug: front-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Webhooks API
  slug: front-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
- filename: front-channel-api-openapi.json
  format: json
  label: Front Channels Platform API
  slug: front-channels-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-channel-api-openapi.json
- filename: front-core-api-openapi.json
  format: json
  label: Front Links API
  slug: front-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/openapi/front-core-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Front Authentication
name_suffix: Authentication
oauth_flows: []
overview: Front secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Front
provider_slug: front
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: http
  scheme: bearer
  sources:
  - openapi/front-channel-api-openapi.json
  - openapi/front-core-api-openapi.json
  type: http
slug: front-authentication
source_filename: front-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/front-channel-api-openapi.json, openapi/front-core-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: http\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/front-channel-api-openapi.json\n  - openapi/front-core-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/front/refs/heads/main/authentication/front-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Support
- Email
- Inbox
- Customer Operations
- Collaboration
- Omnichannel
---
