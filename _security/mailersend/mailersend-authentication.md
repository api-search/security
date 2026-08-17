---
api_key_in:
- header
api_specs:
- filename: mailersend-bulk-email-api-openapi.yml
  format: yaml
  label: MailerSend Bulk Email API
  slug: mailersend-bulk-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-bulk-email-api-openapi.yml
- filename: mailersend-domains-api-openapi.yml
  format: yaml
  label: MailerSend Domains API
  slug: mailersend-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-domains-api-openapi.yml
- filename: mailersend-email-api-openapi.yml
  format: yaml
  label: MailerSend Email API
  slug: mailersend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-email-api-openapi.yml
- filename: mailersend-messages-api-openapi.yml
  format: yaml
  label: MailerSend Messages API
  slug: mailersend-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-messages-api-openapi.yml
- filename: mailersend-sender-identities-api-openapi.yml
  format: yaml
  label: MailerSend Sender Identities API
  slug: mailersend-sender-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-sender-identities-api-openapi.yml
- filename: mailersend-templates-api-openapi.yml
  format: yaml
  label: MailerSend Templates API
  slug: mailersend-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-templates-api-openapi.yml
- filename: mailersend-webhooks-api-openapi.yml
  format: yaml
  label: MailerSend Webhooks API
  slug: mailersend-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mailersend Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MailerSend secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MailerSend
provider_slug: mailersend
scheme_count: 3
schemes:
- description: Long-lived API token generated in the MailerSend dashboard (Settings → API Tokens) or via POST /v1/token. Tokens are issued per sending domain and carry an explicit scope list.
  docs: https://developers.mailersend.com/api/v1/account/tokens
  format: Bearer <API token>
  header: Authorization
  in: header
  name: BearerAuth
  rotation: Tokens can be paused/unpaused (PUT /v1/token/{token_id}) and deleted; no automatic expiry is documented.
  scheme: bearer
  scoped: true
  scopes: scopes/mailersend-scopes.yml
  sources:
  - openapi/_original/mailersend-openapi.yml
  - https://developers.mailersend.com/general
  token_prefix: mlsn.
  type: http
- applies_to: https://mcp.mailersend.com/mcp
  description: OAuth 2.1 authorization server protecting the MailerSend MCP server. Supports RFC 7591 dynamic client registration, PKCE S256, and both authorization_code and refresh_token grants. Discovery via RFC 8414 (/.well-known/oauth-authorization-server) and RFC 9728 (/.well-known/oauth-protected-resource).
  flows:
  - authorizationUrl: https://mcp.mailersend.com/authorize
    flow: authorizationCode
    pkce:
    - S256
    refresh: true
    registrationUrl: https://mcp.mailersend.com/register
    tokenUrl: https://mcp.mailersend.com/token
  name: MCPOAuth
  sources:
  - well-known/mailersend-oauth-authorization-server.json
  - well-known/mailersend-oauth-protected-resource.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- description: SMTP relay users with their own username/password, managed independently of API tokens via the SMTP Users endpoints. Same daily quota and a 120 req/min throttle apply.
  docs: https://developers.mailersend.com/api/v1/email/smtp-relay
  name: SMTPCredentials
  sources:
  - https://developers.mailersend.com/api/v1/account/smtp-users
  type: smtp-basic
slug: mailersend-authentication
source_filename: mailersend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/mailersend-openapi.yml\ndocs: https://developers.mailersend.com/general\nnotes: >-\n  Upgraded from derived to searched on 2026-08-13. The OpenAPI declares a single bearer scheme; the docs\n  add the token model (per-domain, scoped, mlsn.-prefixed), the SMTP credential path, and a second,\n  entirely separate authorization surface — an OAuth 2.1 authorization server fronting the MCP server,\n  which the CLI also uses.\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  api_key_in: [header]\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer <API token>'\n    token_prefix: mlsn.\n    description: >-\n      Long-lived API token generated in the MailerSend dashboard (Settings → API Tokens) or via\n      POST /v1/token. Tokens are issued per sending domain and carry an explicit scope\
  \ list.\n    scoped: true\n    scopes: scopes/mailersend-scopes.yml\n    rotation: 'Tokens can be paused/unpaused (PUT /v1/token/{token_id}) and deleted; no automatic expiry is documented.'\n    docs: https://developers.mailersend.com/api/v1/account/tokens\n    sources:\n      - openapi/_original/mailersend-openapi.yml\n      - https://developers.mailersend.com/general\n  - name: MCPOAuth\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.mailersend.com/authorize\n        tokenUrl: https://mcp.mailersend.com/token\n        registrationUrl: https://mcp.mailersend.com/register\n        refresh: true\n        pkce: [S256]\n    description: >-\n      OAuth 2.1 authorization server protecting the MailerSend MCP server. Supports RFC 7591 dynamic\n      client registration, PKCE S256, and both authorization_code and refresh_token grants. Discovery via\n      RFC 8414 (/.well-known/oauth-authorization-server) and RFC 9728\n      (/.well-known/oauth-protected-resource).\n\
  \    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n    applies_to: https://mcp.mailersend.com/mcp\n    sources:\n      - well-known/mailersend-oauth-authorization-server.json\n      - well-known/mailersend-oauth-protected-resource.json\n  - name: SMTPCredentials\n    type: smtp-basic\n    description: >-\n      SMTP relay users with their own username/password, managed independently of API tokens via the SMTP\n      Users endpoints. Same daily quota and a 120 req/min throttle apply.\n    docs: https://developers.mailersend.com/api/v1/email/smtp-relay\n    sources:\n      - https://developers.mailersend.com/api/v1/account/smtp-users\ncli_authentication:\n  methods: [oauth, api-token]\n  default: oauth\n  commands: ['mailersend auth login', 'mailersend auth login --method token', 'mailersend auth status', 'mailersend auth logout']\n  env_var: MAILERSEND_API_TOKEN\n  resolution_order: 'MAILERSEND_API_TOKEN env var > --profile flag > active profile > first profile'\n\
  \  refresh: 'OAuth tokens are automatically refreshed when they expire.'\n  docs: https://developers.mailersend.com/tools/cli\ncredential_leak_guidance:\n  documented: true\n  url: https://developers.mailersend.com/guides/remediation-of-credential-leaks-api-token-and-smtp\n  note: >-\n    MailerSend publishes a dedicated remediation guide for leaked API tokens and SMTP credentials — an\n    uncommon and genuinely useful piece of operational documentation.\nerrors:\n  '401': The provided API token is invalid.\n  '403': Action denied for the account or the token.\n  MS40301: The custom API token does not have the required permissions.\n  MS40302: The account's API/SMTP access has been switched off by support.\n  MS40305: The requesting IP address is not allowlisted.\nip_allowlisting:\n  supported: true\n  note: Accounts may restrict API access to allowlisted IP addresses; violations return MS40305.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/authentication/mailersend-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Email
- Transactional Email
- SMTP
- Marketing
- Communications
- SMS
- Messaging
- Templates
- Webhooks
- Email Verification
- Deliverability
- Analytics
- MCP
---
