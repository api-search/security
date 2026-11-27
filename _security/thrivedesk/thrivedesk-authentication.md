---
anonymous_access: false
api_key_in: []
api_specs:
- filename: thrivedesk-attachments-api-openapi.yml
  format: yaml
  label: ThriveDesk Attachments API
  slug: thrivedesk-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thrivedesk/openapi/thrivedesk-attachments-api-openapi.yml
- filename: thrivedesk-business-hours-api-openapi.yml
  format: yaml
  label: ThriveDesk Business Hours API
  slug: thrivedesk-business-hours-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thrivedesk/openapi/thrivedesk-business-hours-api-openapi.yml
- filename: thrivedesk-contacts-api-openapi.yml
  format: yaml
  label: ThriveDesk Contacts API
  slug: thrivedesk-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thrivedesk/openapi/thrivedesk-contacts-api-openapi.yml
- filename: thrivedesk-conversations-api-openapi.yml
  format: yaml
  label: ThriveDesk Conversations API
  slug: thrivedesk-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thrivedesk/openapi/thrivedesk-conversations-api-openapi.yml
- filename: thrivedesk-holidays-api-openapi.yml
  format: yaml
  label: ThriveDesk Holidays API
  slug: thrivedesk-holidays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thrivedesk/openapi/thrivedesk-holidays-api-openapi.yml
- filename: thrivedesk-inboxes-api-openapi.yml
  format: yaml
  label: ThriveDesk Inboxes API
  slug: thrivedesk-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thrivedesk/openapi/thrivedesk-inboxes-api-openapi.yml
- filename: thrivedesk-knowledge-base-api-openapi.yml
  format: yaml
  label: ThriveDesk Knowledge Base API
  slug: thrivedesk-knowledge-base-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thrivedesk/openapi/thrivedesk-knowledge-base-api-openapi.yml
- filename: thrivedesk-messages-and-notes-api-openapi.yml
  format: yaml
  label: ThriveDesk Messages and Notes API
  slug: thrivedesk-messages-and-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thrivedesk/openapi/thrivedesk-messages-and-notes-api-openapi.yml
- filename: thrivedesk-misc-api-openapi.yml
  format: yaml
  label: ThriveDesk Misc API
  slug: thrivedesk-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thrivedesk/openapi/thrivedesk-misc-api-openapi.yml
- filename: thrivedesk-reports-api-openapi.yml
  format: yaml
  label: ThriveDesk Reports API
  slug: thrivedesk-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thrivedesk/openapi/thrivedesk-reports-api-openapi.yml
- filename: thrivedesk-saved-replies-api-openapi.yml
  format: yaml
  label: ThriveDesk Saved Replies API
  slug: thrivedesk-saved-replies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thrivedesk/openapi/thrivedesk-saved-replies-api-openapi.yml
- filename: thrivedesk-tags-api-openapi.yml
  format: yaml
  label: ThriveDesk Tags API
  slug: thrivedesk-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thrivedesk/openapi/thrivedesk-tags-api-openapi.yml
- filename: thrivedesk-users-api-openapi.yml
  format: yaml
  label: ThriveDesk Users API
  slug: thrivedesk-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thrivedesk/openapi/thrivedesk-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: ThriveDesk Authentication
name_suffix: Authentication
oauth_flows: []
overview: ThriveDesk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ThriveDesk
provider_slug: thrivedesk
scheme_count: 1
schemes:
- bearerFormat: Personal access token
  description: 'Personal access tokens created from the ThriveDesk UI.

    Create one under Integrations -> API Keys.'
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/thrivedesk-openapi.yml
  type: http
slug: thrivedesk-authentication
source_filename: thrivedesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/thrivedesk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: Personal access token\n  description: |-\n    Personal access tokens created from the ThriveDesk UI.\n    Create one under Integrations -> API Keys.\n  sources:\n  - openapi/thrivedesk-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/thrivedesk/authentication/thrivedesk-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Service
- Artificial Intelligence
- Chatbots
- E-Commerce
- Help Desk
---
