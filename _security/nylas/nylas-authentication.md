---
api_key_in: []
api_specs:
- filename: nylas-api.yaml
  format: yaml
  label: Nylas API
  slug: nylas-api
  spec_type: OpenAPI
  url: https://developer.nylas.com/_spec-files/nylas-api.yaml
- filename: nylas-admin-api-openapi.yml
  format: yaml
  label: Nylas Admin API
  slug: nylas-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-admin-api-openapi.yml
- filename: nylas-auth-api-openapi.yml
  format: yaml
  label: Nylas Auth API
  slug: nylas-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-auth-api-openapi.yml
- filename: nylas-calendars-api-openapi.yml
  format: yaml
  label: Nylas Calendars API
  slug: nylas-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-calendars-api-openapi.yml
- filename: nylas-contacts-api-openapi.yml
  format: yaml
  label: Nylas Contacts API
  slug: nylas-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-contacts-api-openapi.yml
- filename: nylas-drafts-api-openapi.yml
  format: yaml
  label: Nylas Drafts API
  slug: nylas-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-drafts-api-openapi.yml
- filename: nylas-events-api-openapi.yml
  format: yaml
  label: Nylas Events API
  slug: nylas-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-events-api-openapi.yml
- filename: nylas-grants-api-openapi.yml
  format: yaml
  label: Nylas Grants API
  slug: nylas-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-grants-api-openapi.yml
- filename: nylas-messages-api-openapi.yml
  format: yaml
  label: Nylas Messages API
  slug: nylas-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-messages-api-openapi.yml
- filename: nylas-scheduling-api-openapi.yml
  format: yaml
  label: Nylas Scheduling API
  slug: nylas-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-scheduling-api-openapi.yml
- filename: nylas-threads-api-openapi.yml
  format: yaml
  label: Nylas Threads API
  slug: nylas-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-threads-api-openapi.yml
- filename: nylas-notifications-api-openapi.yml
  format: yaml
  label: Nylas Notifications API
  slug: nylas-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-notifications-api-openapi.yml
- filename: nylas-notetaker-api-openapi.yml
  format: yaml
  label: Nylas Notetaker API
  slug: nylas-notetaker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-notetaker-api-openapi.yml
- filename: nylas-templates-workflows-api-openapi.yml
  format: yaml
  label: Nylas Templates and Workflows API
  slug: nylas-templates-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-templates-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: provider-published
name: Nylas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nylas secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nylas
provider_slug: nylas
scheme_count: 3
schemes:
- bearerFormat: NYLAS_API_KEY
  description: Application-level credential covering the application's own resources and all of its grants. Generated in the Nylas Dashboard and presented as a Bearer token. This is the credential used for server-side and machine-to-machine calls, including Agent Accounts, where no browser is available to complete an OAuth flow.
  name: NYLAS_API_KEY
  scheme: bearer
  scope: application
  sources:
  - https://developer.nylas.com/_spec-files/nylas-api.yaml
  type: http
- bearerFormat: NYLAS_ACCESS_TOKEN
  description: Grant-scoped access token issued by the OAuth 2.1 authorization code exchange at POST /v3/connect/token. Used when acting on a single connected end-user mailbox or calendar rather than on the application as a whole.
  name: ACCESS_TOKEN
  scheme: bearer
  scope: grant
  sources:
  - https://developer.nylas.com/_spec-files/nylas-api.yaml
  type: http
- bearerFormat: Session ID
  description: Short-lived Scheduler session ID used by the Scheduler UI Components to authorize booking-flow requests on behalf of an end user without exposing an API key to the browser.
  name: SCHEDULER_SESSION_TOKEN
  scheme: bearer
  scope: session
  sources:
  - https://developer.nylas.com/_spec-files/nylas-api.yaml
  type: http
slug: nylas-authentication
source_filename: nylas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-20'\nmethod: provider-published\nauthored_by: Nylas\nsource: https://developer.nylas.com/_spec-files/nylas-api.yaml\ndocs: https://developer.nylas.com/docs/v3/auth/\nsummary:\n  types:\n  - http\nschemes:\n- name: NYLAS_API_KEY\n  type: http\n  scheme: bearer\n  bearerFormat: NYLAS_API_KEY\n  description: >-\n    Application-level credential covering the application's own resources and\n    all of its grants. Generated in the Nylas Dashboard and presented as a\n    Bearer token. This is the credential used for server-side and\n    machine-to-machine calls, including Agent Accounts, where no browser is\n    available to complete an OAuth flow.\n  scope: application\n  sources:\n  - https://developer.nylas.com/_spec-files/nylas-api.yaml\n- name: ACCESS_TOKEN\n  type: http\n  scheme: bearer\n  bearerFormat: NYLAS_ACCESS_TOKEN\n  description: >-\n    Grant-scoped access token issued by the OAuth 2.1 authorization code\n    exchange at POST /v3/connect/token.\
  \ Used when acting on a single connected\n    end-user mailbox or calendar rather than on the application as a whole.\n  scope: grant\n  sources:\n  - https://developer.nylas.com/_spec-files/nylas-api.yaml\n- name: SCHEDULER_SESSION_TOKEN\n  type: http\n  scheme: bearer\n  bearerFormat: Session ID\n  description: >-\n    Short-lived Scheduler session ID used by the Scheduler UI Components to\n    authorize booking-flow requests on behalf of an end user without exposing an\n    API key to the browser.\n  scope: session\n  sources:\n  - https://developer.nylas.com/_spec-files/nylas-api.yaml\ndefault_security:\n- ACCESS_TOKEN\n- NYLAS_API_KEY\nnotes: >-\n  All three schemes are HTTP Bearer. Security is declared globally in the\n  contract and overridden per operation on 205 of 208 operations. Nylas does not\n  accept credentials in query strings. The previous version of this artifact\n  described a single generic \"BearerAuth\" scheme derived from a summary\n  scaffold; the three schemes\
  \ above are the ones actually declared in the\n  published OpenAPI contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/authentication/nylas-authentication.yml
summary_line: http · 3 schemes
tags:
- Calendar
- Communications
- Contacts
- Email
- Messaging
- Scheduling
---
