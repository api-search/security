---
api_key_in: []
api_specs:
- filename: helpscout-threads-api-openapi.yml
  format: yaml
  label: Help Scout Threads API
  slug: helpscout-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-threads-api-openapi.yml
- filename: helpscout-customers-api-openapi.yml
  format: yaml
  label: Help Scout Customers API
  slug: helpscout-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-customers-api-openapi.yml
- filename: helpscout-mailboxes-api-openapi.yml
  format: yaml
  label: Help Scout Mailboxes API
  slug: helpscout-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-mailboxes-api-openapi.yml
- filename: helpscout-users-api-openapi.yml
  format: yaml
  label: Help Scout Users API
  slug: helpscout-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-users-api-openapi.yml
- filename: helpscout-teams-api-openapi.yml
  format: yaml
  label: Help Scout Teams API
  slug: helpscout-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-teams-api-openapi.yml
- filename: helpscout-tags-api-openapi.yml
  format: yaml
  label: Help Scout Tags API
  slug: helpscout-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-tags-api-openapi.yml
- filename: helpscout-workflows-api-openapi.yml
  format: yaml
  label: Help Scout Workflows API
  slug: helpscout-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-workflows-api-openapi.yml
- filename: helpscout-webhooks-asyncapi.yml
  format: yaml
  label: Help Scout Webhooks API
  slug: helpscout-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/asyncapi/helpscout-webhooks-asyncapi.yml
- filename: helpscout-conversations-api-openapi.yml
  format: yaml
  label: Help Scout Conversations API
  slug: helpscout-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-conversations-api-openapi.yml
- filename: helpscout-customers-api-openapi.yml
  format: yaml
  label: Help Scout Customers API
  slug: helpscout-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-customers-api-openapi.yml
- filename: helpscout-mailboxes-api-openapi.yml
  format: yaml
  label: Help Scout Mailboxes API
  slug: helpscout-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-mailboxes-api-openapi.yml
- filename: helpscout-tags-api-openapi.yml
  format: yaml
  label: Help Scout Tags API
  slug: helpscout-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-tags-api-openapi.yml
- filename: helpscout-teams-api-openapi.yml
  format: yaml
  label: Help Scout Teams API
  slug: helpscout-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-teams-api-openapi.yml
- filename: helpscout-threads-api-openapi.yml
  format: yaml
  label: Help Scout Threads API
  slug: helpscout-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-threads-api-openapi.yml
- filename: helpscout-users-api-openapi.yml
  format: yaml
  label: Help Scout Users API
  slug: helpscout-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-users-api-openapi.yml
- filename: helpscout-webhooks-api-openapi.yml
  format: yaml
  label: Help Scout Webhooks API
  slug: helpscout-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-webhooks-api-openapi.yml
- filename: helpscout-workflows-api-openapi.yml
  format: yaml
  label: Help Scout Workflows API
  slug: helpscout-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-workflows-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Helpscout Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Help Scout secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Help Scout
provider_slug: helpscout
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.helpscout.net/v2/oauth2/token
  name: oauth2
  sources:
  - openapi/helpscout-openapi.yml
  type: oauth2
slug: helpscout-authentication
source_filename: helpscout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/helpscout-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.helpscout.net/v2/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/helpscout-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/authentication/helpscout-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Customer-Support
- Help Desk
- Email
- Live Chat
- Knowledge Base
- Software-as-a-Service
---
