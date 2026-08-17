---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Erxes Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
overview: Erxes secures its APIs with oauth2 and http across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode flow(s).
provider_name: Erxes
provider_slug: erxes
scheme_count: 5
schemes:
- access_token_ttl_seconds: 28800
  client_credentials_required:
  - client_id
  - client_secret
  client_registration: erxes Settings > OAuth Clients (per tenant, in-product)
  client_secret_transport: 'sent as `client_secret` in the OAuth JSON body; the plugin manifest also declares a `clientSecretHeader: oauth_secret`'
  client_type: confidential
  device_code_ttl_seconds: 600
  error_on_missing_secret: invalid_client
  flow: urn:ietf:params:oauth:grant-type:device_code
  name: OAuth2 Device Authorization Grant (confidential client)
  refresh_token: rotating — a new refresh token is issued on every refresh
  rfc: RFC 8628
  sources:
  - https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/erxes-app-token-auth.md
  token_type: Bearer
  type: oauth2
  used_by: erxes-next-plugin (github.com/erxes/erxes-skills)
- client_credentials_required:
  - client_id
  client_type: public
  flow: urn:ietf:params:oauth:grant-type:device_code
  name: OAuth2 Device Authorization Grant (public client)
  note: The CLI requires the OAuth client to explicitly enable the public operations it calls, e.g. core.contacts.customers.list.v1, core.contacts.customers.detail.v1, core.contacts.customers.create.v1.
  rfc: RFC 8628
  sources:
  - https://github.com/erxes/erxes-cli#authenticate
  token_type: Bearer
  type: oauth2
  used_by: erxes CLI (`erxes login --host <gateway> --client-id <id>`)
- applies_to: POST <gateway>/graphql
  header: 'Authorization: Bearer <accessToken>'
  name: Bearer token on GraphQL calls
  scheme: bearer
  sources:
  - https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/erxes-graphql-api.md
  type: http
- applies_to: GraphQL calls only
  in: header
  name: Tenant selector header
  note: NOT a credential — it selects the tenant. erxes explicitly documents that OAuth token and refresh requests must NOT send `erxes-subdomain` (the gateway infers the tenant from the host); the value returned as `subdomain` in the login response is then sent on every GraphQL call. Sending it on the OAuth endpoints is a documented failure mode.
  parameter_name: erxes-subdomain
  required: true
  sources:
  - https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/instructions.md
  type: apiKey
- bearerFormat: JWT
  name: JWT session login (interactive users)
  note: The interactive/app login path, distinct from the machine OAuth device flow above. Documented in graphql/erxes-graphql.md in this repo and in the erxes source.
  obtained_via: '`login` GraphQL mutation (email/password), Google OAuth, or magic link'
  scheme: bearer
  sources:
  - graphql/erxes-graphql.md
  type: http
slug: erxes-authentication
source_filename: erxes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/erxes-app-token-auth.md\ndocs:\n  - https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/erxes-app-token-auth.md\n  - https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/instructions.md\n  - https://github.com/erxes/erxes-cli#authenticate\nnote: >-\n  erxes publishes no OpenAPI, so 0-working/derive-authentication.py produced no\n  profile (0 spec-bearing files). This profile is SEARCHED from the provider's\n  own published agent-plugin auth reference and the first-party CLI README,\n  both of which document the same OAuth 2.0 Device Authorization Grant against\n  the erxes gateway. Two client types are documented and they are not\n  interchangeable: the agent plugin requires a CONFIDENTIAL client (client\n  secret required, sent as `client_secret` in the OAuth JSON body / the\n  `oauth_secret` header), while\
  \ the CLI uses a PUBLIC client (client id only).\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [deviceCode]\n  transport: GraphQL over HTTPS POST\n  multi_tenant: true\nschemes:\n  - name: OAuth2 Device Authorization Grant (confidential client)\n    type: oauth2\n    flow: urn:ietf:params:oauth:grant-type:device_code\n    rfc: RFC 8628\n    client_type: confidential\n    client_credentials_required: [client_id, client_secret]\n    client_secret_transport: >-\n      sent as `client_secret` in the OAuth JSON body; the plugin manifest also\n      declares a `clientSecretHeader: oauth_secret`\n    token_type: Bearer\n    access_token_ttl_seconds: 28800\n    device_code_ttl_seconds: 600\n    refresh_token: rotating — a new refresh token is issued on every refresh\n    error_on_missing_secret: invalid_client\n    client_registration: erxes Settings > OAuth Clients (per tenant, in-product)\n    used_by: erxes-next-plugin (github.com/erxes/erxes-skills)\n    sources:\n\
  \      - https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/erxes-app-token-auth.md\n  - name: OAuth2 Device Authorization Grant (public client)\n    type: oauth2\n    flow: urn:ietf:params:oauth:grant-type:device_code\n    rfc: RFC 8628\n    client_type: public\n    client_credentials_required: [client_id]\n    token_type: Bearer\n    used_by: erxes CLI (`erxes login --host <gateway> --client-id <id>`)\n    note: >-\n      The CLI requires the OAuth client to explicitly enable the public\n      operations it calls, e.g. core.contacts.customers.list.v1,\n      core.contacts.customers.detail.v1, core.contacts.customers.create.v1.\n    sources:\n      - https://github.com/erxes/erxes-cli#authenticate\n  - name: Bearer token on GraphQL calls\n    type: http\n    scheme: bearer\n    header: 'Authorization: Bearer <accessToken>'\n    applies_to: 'POST <gateway>/graphql'\n    sources:\n      - https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/erxes-graphql-api.md\n\
  \  - name: Tenant selector header\n    type: apiKey\n    in: header\n    parameter_name: erxes-subdomain\n    required: true\n    applies_to: GraphQL calls only\n    note: >-\n      NOT a credential — it selects the tenant. erxes explicitly documents that\n      OAuth token and refresh requests must NOT send `erxes-subdomain` (the\n      gateway infers the tenant from the host); the value returned as\n      `subdomain` in the login response is then sent on every GraphQL call.\n      Sending it on the OAuth endpoints is a documented failure mode.\n    sources:\n      - https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/instructions.md\n  - name: JWT session login (interactive users)\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    obtained_via: '`login` GraphQL mutation (email/password), Google OAuth, or magic link'\n    note: >-\n      The interactive/app login path, distinct from the machine OAuth device\n      flow above. Documented in graphql/erxes-graphql.md\
  \ in this repo and in\n      the erxes source.\n    sources:\n      - graphql/erxes-graphql.md\nsession_handling:\n  persistence: >-\n    The erxes agent plugin persists the OAuth session in a home-based state\n    directory (mode 0700 dir / 0600 files) outside the source tree; the CLI\n    stores profile config and credentials separately under the same modes.\n  duration_options: ['3m', '6m', '1y']\n  default_duration: 6m\n  silent_refresh: true\n  session_key: base URL + client id\n  secret_rotation: >-\n    rotating only the client secret keeps the session and is adopted on the\n    next refresh; changing base URL or client id forces a fresh login\nscopes_artifact: scopes/erxes-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erxes/refs/heads/main/authentication/erxes-authentication.yml
summary_line: oauth2/http · 5 schemes
tags:
- GraphQL
- CRM
- Customer Experience
- Open Source
- Marketing Automation
- Sales Pipeline
- Help Desk
- Ticketing
- Team Inbox
- Self-Hosted
- Apollo Federation
- Project Management
- Knowledge Base
- Webhooks
- Agent Skills
---
