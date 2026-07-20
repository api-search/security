---
api_key_in: []
auth_types:
- session
description: ''
kind: authentication
layout: security
method: searched
name: Hansoft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hansoft secures its APIs with session across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hansoft
provider_slug: hansoft
scheme_count: 2
schemes:
- detail: Clients call the `login` mutation to obtain a session before invoking other queries, mutations, or subscriptions. Sessions are scoped to the customer-hosted server and enforce P4 Plan's per-project, field-level permission model.
  name: graphqlLogin
  sources:
  - https://help.perforce.com/hansoft/current/Content/hansoftapi/index.html
  transport: graphql
  type: session
- detail: The native SDK opens a session to the P4 Plan server using the server address, database name, and user credentials (with an SDK primary key / working directory). All SDK operations run in the context of that session.
  name: sdkSession
  sources:
  - https://help.perforce.com/hansoft/sdk/index.html
  transport: sdk
  type: session
slug: hansoft-authentication
source_filename: hansoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://help.perforce.com/hansoft/current/Content/hansoftapi/index.html\ndocs: https://help.perforce.com/hansoft/current/Content/hansoftapi/index.html\nnotes: >-\n  P4 Plan (Hansoft) is not an OpenAPI/OAuth provider. The GraphQL API service\n  authenticates with a login mutation that establishes a session against a\n  customer-hosted P4 Plan server; the native SDK authenticates with a session\n  connection (server address, database, user credentials / SDK primary key).\n  There is no OAuth2 authorization server and no OAuth scope surface, so\n  scopes/ is intentionally skipped.\nsummary:\n  types:\n  - session\n  mechanisms:\n  - graphql-login-mutation\n  - sdk-session\n  oauth2_flows: []\nschemes:\n- name: graphqlLogin\n  type: session\n  transport: graphql\n  detail: >-\n    Clients call the `login` mutation to obtain a session before invoking other\n    queries, mutations, or subscriptions. Sessions are scoped to the\n \
  \   customer-hosted server and enforce P4 Plan's per-project, field-level\n    permission model.\n  sources:\n  - https://help.perforce.com/hansoft/current/Content/hansoftapi/index.html\n- name: sdkSession\n  type: session\n  transport: sdk\n  detail: >-\n    The native SDK opens a session to the P4 Plan server using the server\n    address, database name, and user credentials (with an SDK primary key /\n    working directory). All SDK operations run in the context of that session.\n  sources:\n  - https://help.perforce.com/hansoft/sdk/index.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hansoft/refs/heads/main/authentication/hansoft-authentication.yml
summary_line: session · 2 schemes
tags:
- Company
- Project Management
- Agile
- Planning
- Software Development
- GraphQL
- SDK
- Webhooks
- DevOps
---
