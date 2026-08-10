---
api_key_in:
- header
api_specs:
- filename: chili-piper-availability-api-openapi.yml
  format: yaml
  label: Chili Piper Availability API
  slug: chili-piper-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-availability-api-openapi.yml
- filename: chili-piper-chat-api-openapi.yml
  format: yaml
  label: Chili Piper Chat API
  slug: chili-piper-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-chat-api-openapi.yml
- filename: chili-piper-concierge-api-openapi.yml
  format: yaml
  label: Chili Piper Concierge API
  slug: chili-piper-concierge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-concierge-api-openapi.yml
- filename: chili-piper-distribution-api-openapi.yml
  format: yaml
  label: Chili Piper Distribution API
  slug: chili-piper-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-distribution-api-openapi.yml
- filename: chili-piper-distro-api-openapi.yml
  format: yaml
  label: Chili Piper Distro API
  slug: chili-piper-distro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-distro-api-openapi.yml
- filename: chili-piper-handoff-api-openapi.yml
  format: yaml
  label: Chili Piper Handoff API
  slug: chili-piper-handoff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-handoff-api-openapi.yml
- filename: chili-piper-meeting-type-api-openapi.yml
  format: yaml
  label: Chili Piper Meeting Type API
  slug: chili-piper-meeting-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-meeting-type-api-openapi.yml
- filename: chili-piper-meeting-type-reminder-api-openapi.yml
  format: yaml
  label: Chili Piper Meeting Type Reminder API
  slug: chili-piper-meeting-type-reminder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-meeting-type-reminder-api-openapi.yml
- filename: chili-piper-meetings-api-openapi.yml
  format: yaml
  label: Chili Piper Meetings API
  slug: chili-piper-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-meetings-api-openapi.yml
- filename: chili-piper-rule-api-openapi.yml
  format: yaml
  label: Chili Piper Rule API
  slug: chili-piper-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-rule-api-openapi.yml
- filename: chili-piper-schedulinglinks-api-openapi.yml
  format: yaml
  label: Chili Piper Scheduling Links API
  slug: chili-piper-schedulinglinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-schedulinglinks-api-openapi.yml
- filename: chili-piper-team-api-openapi.yml
  format: yaml
  label: Chili Piper Team API
  slug: chili-piper-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-team-api-openapi.yml
- filename: chili-piper-tenant-api-openapi.yml
  format: yaml
  label: Chili Piper Tenant API
  slug: chili-piper-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-tenant-api-openapi.yml
- filename: chili-piper-user-api-openapi.yml
  format: yaml
  label: Chili Piper User API
  slug: chili-piper-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-user-api-openapi.yml
- filename: chili-piper-workspace-api-openapi.yml
  format: yaml
  label: Chili Piper Workspace API
  slug: chili-piper-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-workspace-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Chili Piper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chili Piper secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chili Piper
provider_slug: chili-piper
scheme_count: 1
schemes:
- description: 'API key in Authorization header. Format: ''Authorization: Bearer <api-key>'' — the word ''Bearer'' followed by a space and the key is required. Sending the key without the Bearer prefix returns 401.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/chili-piper-availability-inspector-openapi.yaml
  - openapi/chili-piper-chat-conversation-inspector-openapi.yaml
  - openapi/chili-piper-concierge-debugger-openapi.yaml
  - openapi/chili-piper-concierge-router-builder-openapi.yaml
  - openapi/chili-piper-concierge-router-configuration-openapi.yaml
  - openapi/chili-piper-distribution-analysis-openapi.yaml
  - openapi/chili-piper-distro-debugger-openapi.yaml
  - openapi/chili-piper-distro-router-configuration-openapi.yaml
  - openapi/chili-piper-handoff-router-configuration-openapi.yaml
  - openapi/chili-piper-meeting-inspector-openapi.yaml
  - openapi/chili-piper-meeting-type-management-openapi.yaml
  - openapi/chili-piper-no-show-analyzer-openapi.yaml
  - openapi/chili-piper-org-meeting-openapi.yaml
  - openapi/chili-piper-routing-audit-openapi.yaml
  - openapi/chili-piper-scheduling-link-management-openapi.yaml
  - openapi/chili-piper-user-copy-openapi.yaml
  - openapi/chili-piper-user-details-openapi.yaml
  - openapi/chili-piper-user-meetings-openapi.yaml
  - openapi/chili-piper-user-offboarding-openapi.yaml
  type: apiKey
slug: chili-piper-authentication
source_filename: chili-piper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: derived\nsource: openapi/chili-piper-availability-inspector-openapi.yaml, openapi/chili-piper-chat-conversation-inspector-openapi.yaml,\n  openapi/chili-piper-concierge-debugger-openapi.yaml, openapi/chili-piper-concierge-router-builder-openapi.yaml,\n  openapi/chili-piper-concierge-router-configuration-openapi.yaml, openapi/chili-piper-distribution-analysis-openapi.yaml,\n  openapi/chili-piper-distro-debugger-openapi.yaml, openapi/chili-piper-distro-router-configuration-openapi.yaml,\n  openapi/chili-piper-handoff-router-configuration-openapi.yaml, openapi/chili-piper-meeting-inspector-openapi.yaml,\n  openapi/chili-piper-meeting-type-management-openapi.yaml, openapi/chili-piper-no-show-analyzer-openapi.yaml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key in Authorization header. Format: ''Authorization: Bearer\
  \ <api-key>''\n    — the word ''Bearer'' followed by a space and the key is required. Sending the key without\n    the Bearer prefix returns 401.'\n  sources:\n  - openapi/chili-piper-availability-inspector-openapi.yaml\n  - openapi/chili-piper-chat-conversation-inspector-openapi.yaml\n  - openapi/chili-piper-concierge-debugger-openapi.yaml\n  - openapi/chili-piper-concierge-router-builder-openapi.yaml\n  - openapi/chili-piper-concierge-router-configuration-openapi.yaml\n  - openapi/chili-piper-distribution-analysis-openapi.yaml\n  - openapi/chili-piper-distro-debugger-openapi.yaml\n  - openapi/chili-piper-distro-router-configuration-openapi.yaml\n  - openapi/chili-piper-handoff-router-configuration-openapi.yaml\n  - openapi/chili-piper-meeting-inspector-openapi.yaml\n  - openapi/chili-piper-meeting-type-management-openapi.yaml\n  - openapi/chili-piper-no-show-analyzer-openapi.yaml\n  - openapi/chili-piper-org-meeting-openapi.yaml\n  - openapi/chili-piper-routing-audit-openapi.yaml\n \
  \ - openapi/chili-piper-scheduling-link-management-openapi.yaml\n  - openapi/chili-piper-user-copy-openapi.yaml\n  - openapi/chili-piper-user-details-openapi.yaml\n  - openapi/chili-piper-user-meetings-openapi.yaml\n  - openapi/chili-piper-user-offboarding-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/authentication/chili-piper-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Scheduling
- Lead Routing
- Meetings
- Sales
- Marketing
- CRM
- Demand Conversion
- Appointment Booking
- Revenue Operations
- Calendar
- Agents
- MCP
---
