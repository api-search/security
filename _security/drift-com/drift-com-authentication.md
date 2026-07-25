---
api_key_in: []
api_specs:
- filename: drift-com-accounts-api-openapi.yml
  format: yaml
  label: Drift Accounts API
  slug: drift-com-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-accounts-api-openapi.yml
- filename: drift-com-app-admin-api-openapi.yml
  format: yaml
  label: Drift App Admin API
  slug: drift-com-app-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-app-admin-api-openapi.yml
- filename: drift-com-contacts-api-openapi.yml
  format: yaml
  label: Drift Contacts API
  slug: drift-com-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-contacts-api-openapi.yml
- filename: drift-com-conversations-and-messages-api-openapi.yml
  format: yaml
  label: Drift Conversations and Messages API
  slug: drift-com-conversations-and-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-conversations-and-messages-api-openapi.yml
- filename: drift-com-data-privacy-api-openapi.yml
  format: yaml
  label: Drift Data Privacy API
  slug: drift-com-data-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-data-privacy-api-openapi.yml
- filename: drift-com-playbooks-api-openapi.yml
  format: yaml
  label: Drift Playbooks API
  slug: drift-com-playbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-playbooks-api-openapi.yml
- filename: drift-com-scim-api-api-openapi.yml
  format: yaml
  label: Drift SCIM API API
  slug: drift-com-scim-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-scim-api-api-openapi.yml
- filename: drift-com-teams-api-openapi.yml
  format: yaml
  label: Drift Teams API
  slug: drift-com-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-teams-api-openapi.yml
- filename: drift-com-users-api-openapi.yml
  format: yaml
  label: Drift Users API
  slug: drift-com-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Drift Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drift secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Drift
provider_slug: drift-com
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/drift-com-openapi.yml
  type: http
slug: drift-com-authentication
source_filename: drift-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drift-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/drift-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/authentication/drift-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Conversational Marketing
- Chatbots
- Sales
- Messaging
- Customer Engagement
- Revenue Orchestration
- AI Chat
---
