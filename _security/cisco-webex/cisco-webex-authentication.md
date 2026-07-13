---
api_key_in: []
api_specs:
- filename: cisco-webex-meetings-openapi.yml
  format: yaml
  label: Webex Meetings API
  slug: webex-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-meetings-openapi.yml
- filename: cisco-webex-messaging-openapi.yml
  format: yaml
  label: Webex Messaging API
  slug: webex-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-messaging-openapi.yml
- filename: cisco-webex-people-openapi.yml
  format: yaml
  label: Webex People API
  slug: webex-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-people-openapi.yml
- filename: cisco-webex-teams-openapi.yml
  format: yaml
  label: Webex Teams API
  slug: webex-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-teams-openapi.yml
- filename: cisco-webex-rooms-openapi.yml
  format: yaml
  label: Webex Rooms API
  slug: webex-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-rooms-openapi.yml
- filename: cisco-webex-webhooks-openapi.yml
  format: yaml
  label: Webex Webhooks API
  slug: webex-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-webhooks-openapi.yml
- filename: cisco-webex-devices-openapi.yml
  format: yaml
  label: Webex Devices API
  slug: webex-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-devices-openapi.yml
- filename: cisco-webex-memberships-openapi.yml
  format: yaml
  label: Webex Memberships API
  slug: webex-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-memberships-openapi.yml
- filename: cisco-webex-team-memberships-openapi.yml
  format: yaml
  label: Webex Team Memberships API
  slug: webex-team-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-team-memberships-openapi.yml
- filename: cisco-webex-events-openapi.yml
  format: yaml
  label: Webex Events API
  slug: webex-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-events-openapi.yml
- filename: cisco-webex-recordings-openapi.yml
  format: yaml
  label: Webex Recordings API
  slug: webex-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-recordings-openapi.yml
- filename: cisco-webex-call-controls-openapi.yml
  format: yaml
  label: Webex Call Controls API
  slug: webex-call-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-call-controls-openapi.yml
- filename: cisco-webex-attachment-actions-openapi.yml
  format: yaml
  label: Webex Attachment Actions API
  slug: webex-attachment-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-attachment-actions-openapi.yml
- filename: cisco-webex-organizations-openapi.yml
  format: yaml
  label: Webex Organizations API
  slug: webex-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-organizations-openapi.yml
- filename: cisco-webex-licenses-openapi.yml
  format: yaml
  label: Webex Licenses API
  slug: webex-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-licenses-openapi.yml
- filename: cisco-webex-roles-openapi.yml
  format: yaml
  label: Webex Roles API
  slug: webex-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-roles-openapi.yml
- filename: cisco-webex-workspaces-openapi.yml
  format: yaml
  label: Webex Workspaces API
  slug: webex-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-workspaces-openapi.yml
- filename: cisco-webex-admin-audit-events-openapi.yml
  format: yaml
  label: Webex Admin Audit Events API
  slug: webex-admin-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-admin-audit-events-openapi.yml
- filename: cisco-webex-converged-recordings-openapi.yml
  format: yaml
  label: Webex Converged Recordings API
  slug: webex-converged-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-converged-recordings-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Webex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Webex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cisco Webex
provider_slug: cisco-webex
scheme_count: 1
schemes:
- description: Webex API access token. Obtain via OAuth 2.0 authorization flow. Requires audit:events_read scope.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cisco-webex-admin-audit-events-openapi.yml
  - openapi/cisco-webex-attachment-actions-openapi.yml
  - openapi/cisco-webex-call-controls-openapi.yml
  - openapi/cisco-webex-converged-recordings-openapi.yml
  - openapi/cisco-webex-devices-openapi.yml
  - openapi/cisco-webex-events-openapi.yml
  - openapi/cisco-webex-licenses-openapi.yml
  - openapi/cisco-webex-meetings-openapi.yml
  - openapi/cisco-webex-memberships-openapi.yml
  - openapi/cisco-webex-messaging-openapi.yml
  - openapi/cisco-webex-organizations-openapi.yml
  - openapi/cisco-webex-people-openapi.yml
  - openapi/cisco-webex-recordings-openapi.yml
  - openapi/cisco-webex-roles-openapi.yml
  - openapi/cisco-webex-rooms-openapi.yml
  - openapi/cisco-webex-team-memberships-openapi.yml
  - openapi/cisco-webex-teams-openapi.yml
  - openapi/cisco-webex-webhooks-openapi.yml
  - openapi/cisco-webex-workspaces-openapi.yml
  type: http
slug: cisco-webex-authentication
source_filename: cisco-webex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-webex-admin-audit-events-openapi.yml, openapi/cisco-webex-attachment-actions-openapi.yml,\n  openapi/cisco-webex-call-controls-openapi.yml, openapi/cisco-webex-converged-recordings-openapi.yml,\n  openapi/cisco-webex-devices-openapi.yml, openapi/cisco-webex-events-openapi.yml, openapi/cisco-webex-licenses-openapi.yml,\n  openapi/cisco-webex-meetings-openapi.yml, openapi/cisco-webex-memberships-openapi.yml, openapi/cisco-webex-messaging-openapi.yml,\n  openapi/cisco-webex-organizations-openapi.yml, openapi/cisco-webex-people-openapi.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Webex API access token. Obtain via OAuth 2.0 authorization flow. Requires audit:events_read\n    scope.\n  sources:\n  - openapi/cisco-webex-admin-audit-events-openapi.yml\n  - openapi/cisco-webex-attachment-actions-openapi.yml\n  - openapi/cisco-webex-call-controls-openapi.yml\n\
  \  - openapi/cisco-webex-converged-recordings-openapi.yml\n  - openapi/cisco-webex-devices-openapi.yml\n  - openapi/cisco-webex-events-openapi.yml\n  - openapi/cisco-webex-licenses-openapi.yml\n  - openapi/cisco-webex-meetings-openapi.yml\n  - openapi/cisco-webex-memberships-openapi.yml\n  - openapi/cisco-webex-messaging-openapi.yml\n  - openapi/cisco-webex-organizations-openapi.yml\n  - openapi/cisco-webex-people-openapi.yml\n  - openapi/cisco-webex-recordings-openapi.yml\n  - openapi/cisco-webex-roles-openapi.yml\n  - openapi/cisco-webex-rooms-openapi.yml\n  - openapi/cisco-webex-team-memberships-openapi.yml\n  - openapi/cisco-webex-teams-openapi.yml\n  - openapi/cisco-webex-webhooks-openapi.yml\n  - openapi/cisco-webex-workspaces-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/authentication/cisco-webex-authentication.yml
summary_line: http · 1 scheme
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
---
