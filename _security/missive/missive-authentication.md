---
api_key_in: []
api_specs:
- filename: missive-analytics-api-openapi.yml
  format: yaml
  label: Missive Analytics API
  slug: missive-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/missive/refs/heads/main/openapi/missive-analytics-api-openapi.yml
- filename: missive-contact-books-api-openapi.yml
  format: yaml
  label: Missive Contact Books API
  slug: missive-contact-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/missive/refs/heads/main/openapi/missive-contact-books-api-openapi.yml
- filename: missive-contact-groups-api-openapi.yml
  format: yaml
  label: Missive Contact Groups API
  slug: missive-contact-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/missive/refs/heads/main/openapi/missive-contact-groups-api-openapi.yml
- filename: missive-contacts-api-openapi.yml
  format: yaml
  label: Missive Contacts API
  slug: missive-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/missive/refs/heads/main/openapi/missive-contacts-api-openapi.yml
- filename: missive-conversations-api-openapi.yml
  format: yaml
  label: Missive Conversations API
  slug: missive-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/missive/refs/heads/main/openapi/missive-conversations-api-openapi.yml
- filename: missive-drafts-api-openapi.yml
  format: yaml
  label: Missive Drafts API
  slug: missive-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/missive/refs/heads/main/openapi/missive-drafts-api-openapi.yml
- filename: missive-messages-api-openapi.yml
  format: yaml
  label: Missive Messages API
  slug: missive-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/missive/refs/heads/main/openapi/missive-messages-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Missive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Missive secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Missive
provider_slug: missive
scheme_count: 1
schemes:
- description: 'Personal access token generated in Missive preferences. Format: Bearer [example key][token]. Requires Productive plan or higher.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/missive-rest-api-openapi.yml
  type: http
slug: missive-authentication
source_filename: missive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/missive-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Personal access token generated in Missive preferences. Format: Bearer [example key][token].\n    Requires Productive plan or higher.'\n  sources:\n  - openapi/missive-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/missive/refs/heads/main/authentication/missive-authentication.yml
summary_line: http · 1 scheme
tags:
- Team Inbox
- Collaboration
- Email
- Messaging
- Conversations
- Contacts
- Webhook
- Automation
- REST API
---
