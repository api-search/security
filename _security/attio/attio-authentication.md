---
api_key_in: []
api_specs:
- filename: attio-attributes-api-openapi.yml
  format: yaml
  label: Attio Attributes API
  slug: attio-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-attributes-api-openapi.yml
- filename: attio-call-recordings-api-openapi.yml
  format: yaml
  label: Attio Call Recordings API
  slug: attio-call-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-call-recordings-api-openapi.yml
- filename: attio-comments-api-openapi.yml
  format: yaml
  label: Attio Comments API
  slug: attio-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-comments-api-openapi.yml
- filename: attio-entries-api-openapi.yml
  format: yaml
  label: Attio Entries API
  slug: attio-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-entries-api-openapi.yml
- filename: attio-files-api-openapi.yml
  format: yaml
  label: Attio Files API
  slug: attio-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-files-api-openapi.yml
- filename: attio-lists-api-openapi.yml
  format: yaml
  label: Attio Lists API
  slug: attio-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-lists-api-openapi.yml
- filename: attio-meetings-api-openapi.yml
  format: yaml
  label: Attio Meetings API
  slug: attio-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-meetings-api-openapi.yml
- filename: attio-meta-api-openapi.yml
  format: yaml
  label: Attio Meta API
  slug: attio-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-meta-api-openapi.yml
- filename: attio-notes-api-openapi.yml
  format: yaml
  label: Attio Notes API
  slug: attio-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-notes-api-openapi.yml
- filename: attio-oauth-api-openapi.yml
  format: yaml
  label: Attio OAuth API
  slug: attio-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-oauth-api-openapi.yml
- filename: attio-objects-api-openapi.yml
  format: yaml
  label: Attio Objects API
  slug: attio-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-objects-api-openapi.yml
- filename: attio-records-api-openapi.yml
  format: yaml
  label: Attio Records API
  slug: attio-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-records-api-openapi.yml
- filename: attio-tasks-api-openapi.yml
  format: yaml
  label: Attio Tasks API
  slug: attio-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-tasks-api-openapi.yml
- filename: attio-threads-api-openapi.yml
  format: yaml
  label: Attio Threads API
  slug: attio-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-threads-api-openapi.yml
- filename: attio-webhooks-api-openapi.yml
  format: yaml
  label: Attio Webhooks API
  slug: attio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-webhooks-api-openapi.yml
- filename: attio-workspace-members-api-openapi.yml
  format: yaml
  label: Attio Workspace Members API
  slug: attio-workspace-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/openapi/attio-workspace-members-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Attio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Attio secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Attio
provider_slug: attio
scheme_count: 2
schemes:
- description: Attio API key or OAuth bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/attio-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://app.attio.com/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://api.attio.com/oauth/token
  name: oauth2
  sources:
  - openapi/attio-openapi.yml
  type: oauth2
slug: attio-authentication
source_filename: attio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/attio-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Attio API key or OAuth bearer token.\n  sources:\n  - openapi/attio-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.attio.com/authorize\n    tokenUrl: https://api.attio.com/oauth/token\n    scopes: 7\n  sources:\n  - openapi/attio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/authentication/attio-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- CRM
- Customer Relationship Management
- Sales
- Contacts
- Companies
- Pipeline
- Workflows
---
