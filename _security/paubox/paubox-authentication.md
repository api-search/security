---
api_key_in:
- header
api_specs:
- filename: paubox-analytics-api-openapi.yml
  format: yaml
  label: Paubox Analytics API
  slug: paubox-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-analytics-api-openapi.yml
- filename: paubox-campaign-mailings-api-openapi.yml
  format: yaml
  label: Paubox Campaign Mailings API
  slug: paubox-campaign-mailings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-campaign-mailings-api-openapi.yml
- filename: paubox-drip-campaigns-api-openapi.yml
  format: yaml
  label: Paubox Drip Campaigns API
  slug: paubox-drip-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-drip-campaigns-api-openapi.yml
- filename: paubox-dynamic-templates-api-openapi.yml
  format: yaml
  label: Paubox Dynamic Templates API
  slug: paubox-dynamic-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-dynamic-templates-api-openapi.yml
- filename: paubox-form-management-api-openapi.yml
  format: yaml
  label: Paubox Form management API
  slug: paubox-form-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-form-management-api-openapi.yml
- filename: paubox-forms-api-openapi.yml
  format: yaml
  label: Paubox Forms API
  slug: paubox-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-forms-api-openapi.yml
- filename: paubox-messages-api-openapi.yml
  format: yaml
  label: Paubox Messages API
  slug: paubox-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-messages-api-openapi.yml
- filename: paubox-submissions-api-openapi.yml
  format: yaml
  label: Paubox Submissions API
  slug: paubox-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-submissions-api-openapi.yml
- filename: paubox-subscribers-api-openapi.yml
  format: yaml
  label: Paubox Subscribers API
  slug: paubox-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-subscribers-api-openapi.yml
- filename: paubox-subscription-lists-api-openapi.yml
  format: yaml
  label: Paubox Subscription Lists API
  slug: paubox-subscription-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-subscription-lists-api-openapi.yml
- filename: paubox-subscriptions-api-openapi.yml
  format: yaml
  label: Paubox Subscriptions API
  slug: paubox-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-subscriptions-api-openapi.yml
- filename: paubox-tracking-links-api-openapi.yml
  format: yaml
  label: Paubox Tracking Links API
  slug: paubox-tracking-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-tracking-links-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: 'Paubox authenticates with static API keys issued per verified sending domain. There is no OAuth on any of the three REST APIs — OAuth 2.1 exists only in front of the MCP server. The header FORMAT differs between products, which is the most common integration mistake: Bearer for Email and Forms, `Token token=` for Marketing.'
kind: authentication
layout: security
method: searched
name: Paubox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paubox secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Paubox
provider_slug: paubox
scheme_count: 5
schemes:
- api: Paubox Email API
  docs: https://docs.paubox.com/email-api/authentication
  format: 'Authorization: Bearer YOUR_API_KEY'
  legacy_format: 'Authorization: Token token=YOUR_API_KEY'
  legacy_note: Still accepted; provider states Bearer is preferred for new integrations.
  location: Authorization header
  name: PauboxToken
  scheme: bearer
  sources:
  - openapi/paubox-email-api-openapi.yaml
  type: http
- api: Paubox Forms API
  docs: https://docs.paubox.com/forms/authentication
  format: 'Authorization: Bearer YOUR_API_KEY'
  location: Authorization header
  name: bearerAuth
  note: The Forms API does NOT accept the `Token token=` format. Two operations — getPublicForm and createFormSubmission — take no credential at all; the form UUID is the access control.
  required_scope: forms
  scheme: bearer
  sources:
  - openapi/paubox-forms-api-openapi.yaml
  type: http
- api: Paubox Marketing API
  docs: https://docs.paubox.com/marketing
  format: 'Authorization: Token token=<API_KEY>'
  in: header
  name: TokenAuth
  note: Bearer is not documented for Marketing. Marketing is a separately purchased plan, so an Email API key will not necessarily work here.
  parameter: authorization
  sources:
  - openapi/paubox-marketing-api-openapi.yaml
  type: apiKey
- api: Paubox Email API (SMTP transport)
  docs: https://docs.paubox.com/email-api/smtp
  host: smtp.paubox.com
  name: SMTP
  password: your Paubox API key
  port: 587
  scheme: basic
  type: http
  username: apikey
- alternatives:
  - 'x-paubox-api-key: <api key> request header'
  - PAUBOX_API_KEY environment variable (stdio transport)
  - optional apiKey parameter on every tool (HTTP transport only)
  api: Paubox MCP Server
  authorization_endpoint: https://mcp.paubox.com/oauth/authorize
  code_challenge_methods_supported:
  - S256
  discovery: well-known/paubox-mcp-oauth-authorization-server.json
  docs: https://docs.paubox.com/mcp-server/authentication
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.paubox.com
  name: MCP OAuth
  registration_endpoint: https://mcp.paubox.com/register
  response_types_supported:
  - code
  scopes_note: The authorization-server metadata declares NO scopes_supported, so there is no published OAuth scope vocabulary. This is why no scopes/ artifact is emitted.
  scopes_supported: null
  token_endpoint: https://mcp.paubox.com/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: paubox-authentication
source_filename: paubox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://docs.paubox.com/email-api/authentication,\n  https://docs.paubox.com/forms/authentication, https://docs.paubox.com/marketing,\n  https://docs.paubox.com/mcp-server/authentication and\n  https://docs.paubox.com/email-api/smtp — cross-checked against the securitySchemes\n  declared in the three OpenAPI documents under openapi/.\ndescription: >-\n  Paubox authenticates with static API keys issued per verified sending domain. There is\n  no OAuth on any of the three REST APIs — OAuth 2.1 exists only in front of the MCP\n  server. The header FORMAT differs between products, which is the most common\n  integration mistake: Bearer for Email and Forms, `Token token=` for Marketing.\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2_scope: mcp-server-only\n  key_issuance: Paubox dashboard, per verified sending domain. Displayed once at creation.\n  key_scoping: >-\n    Keys are scoped per product.\
  \ A key scoped only to the Email API is rejected by the\n    Forms API with 401.\n\nschemes:\n  - name: PauboxToken\n    api: Paubox Email API\n    type: http\n    scheme: bearer\n    location: 'Authorization header'\n    format: 'Authorization: Bearer YOUR_API_KEY'\n    legacy_format: 'Authorization: Token token=YOUR_API_KEY'\n    legacy_note: Still accepted; provider states Bearer is preferred for new integrations.\n    docs: https://docs.paubox.com/email-api/authentication\n    sources:\n      - openapi/paubox-email-api-openapi.yaml\n  - name: bearerAuth\n    api: Paubox Forms API\n    type: http\n    scheme: bearer\n    location: 'Authorization header'\n    format: 'Authorization: Bearer YOUR_API_KEY'\n    required_scope: forms\n    docs: https://docs.paubox.com/forms/authentication\n    note: >-\n      The Forms API does NOT accept the `Token token=` format. Two operations —\n      getPublicForm and createFormSubmission — take no credential at all; the form UUID is\n      the access\
  \ control.\n    sources:\n      - openapi/paubox-forms-api-openapi.yaml\n  - name: TokenAuth\n    api: Paubox Marketing API\n    type: apiKey\n    in: header\n    parameter: authorization\n    format: 'Authorization: Token token=<API_KEY>'\n    docs: https://docs.paubox.com/marketing\n    note: >-\n      Bearer is not documented for Marketing. Marketing is a separately purchased plan, so\n      an Email API key will not necessarily work here.\n    sources:\n      - openapi/paubox-marketing-api-openapi.yaml\n  - name: SMTP\n    api: Paubox Email API (SMTP transport)\n    type: http\n    scheme: basic\n    host: smtp.paubox.com\n    port: 587\n    username: apikey\n    password: your Paubox API key\n    docs: https://docs.paubox.com/email-api/smtp\n  - name: MCP OAuth\n    api: Paubox MCP Server\n    type: oauth2\n    issuer: https://mcp.paubox.com\n    authorization_endpoint: https://mcp.paubox.com/oauth/authorize\n    token_endpoint: https://mcp.paubox.com/oauth/token\n    registration_endpoint:\
  \ https://mcp.paubox.com/register\n    response_types_supported: [code]\n    grant_types_supported: [authorization_code, refresh_token]\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [none]\n    scopes_supported: null\n    scopes_note: >-\n      The authorization-server metadata declares NO scopes_supported, so there is no\n      published OAuth scope vocabulary. This is why no scopes/ artifact is emitted.\n    alternatives:\n      - 'x-paubox-api-key: <api key> request header'\n      - PAUBOX_API_KEY environment variable (stdio transport)\n      - optional apiKey parameter on every tool (HTTP transport only)\n    docs: https://docs.paubox.com/mcp-server/authentication\n    discovery: well-known/paubox-mcp-oauth-authorization-server.json\n\nkey_management:\n  rotation: >-\n    Each domain can hold multiple active keys, so rotation is: create the new key, cut\n    traffic over, then revoke the old one.\n  revocation: Provider advises immediate\
  \ revocation on exposure or staff departure.\n  storage_guidance: >-\n    Provider warns against committing keys to source control and recommends environment\n    variables or a secrets manager. The CLI stores credentials in the OS keychain, falling\n    back to ~/.config/paubox/config.json at 0600.\n\ngaps:\n  - No OAuth, no scopes and no token exchange on any of the three REST APIs.\n  - >-\n    No scope vocabulary published for the MCP OAuth server either — scopes_supported is\n    absent from the authorization-server metadata.\n  - >-\n    Three different header conventions across three APIs on one host, with no shared\n    documentation page reconciling them.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/authentication/paubox-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Email
- HIPAA
- Healthcare
- Compliance
- Transactional Email
- Email Marketing
- Forms
- Security
- Encryption
- Messaging
---
