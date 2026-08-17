---
api_key_in: []
api_specs:
- filename: snov-io-authentication-api-openapi.yml
  format: yaml
  label: Snov.io Authentication API
  slug: snov-io-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-authentication-api-openapi.yml
- filename: snov-io-campaigns-api-openapi.yml
  format: yaml
  label: Snov.io Campaigns API
  slug: snov-io-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-campaigns-api-openapi.yml
- filename: snov-io-crm-pipeline-api-openapi.yml
  format: yaml
  label: Snov.io CRM Pipeline API
  slug: snov-io-crm-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-crm-pipeline-api-openapi.yml
- filename: snov-io-domain-search-api-openapi.yml
  format: yaml
  label: Snov.io Domain Search API
  slug: snov-io-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-domain-search-api-openapi.yml
- filename: snov-io-email-accounts-api-openapi.yml
  format: yaml
  label: Snov.io Email Accounts API
  slug: snov-io-email-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-accounts-api-openapi.yml
- filename: snov-io-email-finder-api-openapi.yml
  format: yaml
  label: Snov.io Email Finder API
  slug: snov-io-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-finder-api-openapi.yml
- filename: snov-io-email-verification-api-openapi.yml
  format: yaml
  label: Snov.io Email Verification API
  slug: snov-io-email-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-verification-api-openapi.yml
- filename: snov-io-email-warm-up-api-openapi.yml
  format: yaml
  label: Snov.io Email Warm-up API
  slug: snov-io-email-warm-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-warm-up-api-openapi.yml
- filename: snov-io-prospects-api-openapi.yml
  format: yaml
  label: Snov.io Prospects API
  slug: snov-io-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-prospects-api-openapi.yml
- filename: snov-io-user-api-openapi.yml
  format: yaml
  label: Snov.io User API
  slug: snov-io-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-user-api-openapi.yml
- filename: snov-io-webhooks-api-openapi.yml
  format: yaml
  label: Snov.io Webhooks API
  slug: snov-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-webhooks-api-openapi.yml
auth_types:
- oauth2
- http
description: Snov.io runs TWO independent OAuth 2.0 deployments that share no credentials, no host and no grant type. The REST API at api.snov.io uses client_credentials to mint a 3600-second Bearer token from an API user id and secret the account holder copies out of the web app. The remote MCP server at mcp.snov.io uses authorization_code with PKCE against an authorization server on app.snov.io, with open dynamic client registration and a single scope named "mcp". A token minted for one will not work on the other.
kind: authentication
layout: security
method: searched
name: Snov Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snov.io secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Snov.io
provider_slug: snov-io
scheme_count: 3
schemes:
- flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  note: No scope parameter is accepted and no scopes are issued. Authorization is entirely plan-derived — what a token can do is decided by the account's subscription tier and credit balance, not by the credential. Re-POST the token endpoint to renew; there is no refresh grant.
  parameters:
  - name: grant_type
    required: true
    value: client_credentials
  - description: API User ID, from https://app.snov.io/account/api
    name: client_id
    required: true
  - description: API Secret, from https://app.snov.io/account/api
    name: client_secret
    required: true
  refresh_token: false
  response_fields:
  - access_token
  - token_type
  - expires_in
  scopes: []
  sources:
  - https://snov.io/api
  - openapi/snov-io-authentication-api-openapi.yml
  surface: REST API
  token_ttl_seconds: 3600
  token_url: https://api.snov.io/v1/oauth/access_token
  type: oauth2
- description: The token returned by the client_credentials exchange, presented on every subsequent REST call. Snov.io's own examples show a small number of legacy v1 endpoints accepting the token as an `access_token` form field instead of a header — prefer the header everywhere.
  header: 'Authorization: Bearer <access_token>'
  name: BearerToken
  scheme: bearer
  sources:
  - https://snov.io/api
  surface: REST API
  type: http
- authorization_endpoint: https://app.snov.io/mcp/authorize
  authorization_server: https://app.snov.io
  bearer_methods_supported:
  - header
  dynamic_client_registration: true
  flow: authorizationCode
  grant_types_supported:
  - authorization_code
  - refresh_token
  name: OAuth2AuthorizationCodeMCP
  note: 'Public-client OAuth: no client secret, PKCE required, and open RFC 7591 dynamic registration so an MCP client can self-register. The user approves the connection inside their Snov.io account, which is why Snov.io can say "you never share raw API keys" with an AI assistant. Unlike the REST surface, this flow DOES issue refresh tokens.'
  pkce: S256
  registration_endpoint: https://app.snov.io/back/mcp/oauth/register
  resource: https://mcp.snov.io/mcp
  scopes:
  - description: The only scope Snov.io issues. Grants an MCP client the full published action surface — prospecting, email verification, Sales CRM and LinkedIn outreach — with no finer-grained separation between read and write.
    name: mcp
  sources:
  - https://mcp.snov.io/.well-known/oauth-protected-resource
  - https://app.snov.io/.well-known/oauth-authorization-server
  - https://snov.io/knowledgebase/how-to-use-snov-io-mcp-with-your-ai-assistant/
  surface: MCP server
  token_endpoint: https://app.snov.io/back/mcp/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: snov-io-authentication
source_filename: snov-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://snov.io/api\ndocs: https://snov.io/knowledgebase/how-to-use-snov-io-api/\ndescription: >-\n  Snov.io runs TWO independent OAuth 2.0 deployments that share no credentials, no host and no\n  grant type. The REST API at api.snov.io uses client_credentials to mint a 3600-second Bearer\n  token from an API user id and secret the account holder copies out of the web app. The remote\n  MCP server at mcp.snov.io uses authorization_code with PKCE against an authorization server on\n  app.snov.io, with open dynamic client registration and a single scope named \"mcp\". A token\n  minted for one will not work on the other.\nsummary:\n  types:\n    - oauth2\n    - http\n  surfaces: 2\n  mfa_for_api: false\n  api_keys: false\n\nschemes:\n  - name: OAuth2ClientCredentials\n    surface: REST API\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://api.snov.io/v1/oauth/access_token\n    grant_type: client_credentials\n\
  \    parameters:\n      - name: grant_type\n        value: client_credentials\n        required: true\n      - name: client_id\n        description: API User ID, from https://app.snov.io/account/api\n        required: true\n      - name: client_secret\n        description: API Secret, from https://app.snov.io/account/api\n        required: true\n    response_fields:\n      - access_token\n      - token_type\n      - expires_in\n    token_ttl_seconds: 3600\n    refresh_token: false\n    scopes: []\n    note: >-\n      No scope parameter is accepted and no scopes are issued. Authorization is entirely\n      plan-derived — what a token can do is decided by the account's subscription tier and\n      credit balance, not by the credential. Re-POST the token endpoint to renew; there is no\n      refresh grant.\n    sources:\n      - https://snov.io/api\n      - openapi/snov-io-authentication-api-openapi.yml\n\n  - name: BearerToken\n    surface: REST API\n    type: http\n    scheme: bearer\n\
  \    header: 'Authorization: Bearer <access_token>'\n    description: >-\n      The token returned by the client_credentials exchange, presented on every subsequent REST\n      call. Snov.io's own examples show a small number of legacy v1 endpoints accepting the\n      token as an `access_token` form field instead of a header — prefer the header everywhere.\n    sources:\n      - https://snov.io/api\n\n  - name: OAuth2AuthorizationCodeMCP\n    surface: MCP server\n    type: oauth2\n    flow: authorizationCode\n    resource: https://mcp.snov.io/mcp\n    authorization_server: https://app.snov.io\n    authorization_endpoint: https://app.snov.io/mcp/authorize\n    token_endpoint: https://app.snov.io/back/mcp/oauth/token\n    registration_endpoint: https://app.snov.io/back/mcp/oauth/register\n    pkce: S256\n    dynamic_client_registration: true\n    token_endpoint_auth_methods_supported:\n      - none\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n    bearer_methods_supported:\n\
  \      - header\n    scopes:\n      - name: mcp\n        description: >-\n          The only scope Snov.io issues. Grants an MCP client the full published action surface\n          — prospecting, email verification, Sales CRM and LinkedIn outreach — with no\n          finer-grained separation between read and write.\n    note: >-\n      Public-client OAuth: no client secret, PKCE required, and open RFC 7591 dynamic\n      registration so an MCP client can self-register. The user approves the connection inside\n      their Snov.io account, which is why Snov.io can say \"you never share raw API keys\" with\n      an AI assistant. Unlike the REST surface, this flow DOES issue refresh tokens.\n    sources:\n      - https://mcp.snov.io/.well-known/oauth-protected-resource\n      - https://app.snov.io/.well-known/oauth-authorization-server\n      - https://snov.io/knowledgebase/how-to-use-snov-io-mcp-with-your-ai-assistant/\n\ncredential_management:\n  console: https://app.snov.io/account/api\n\
  \  rotation_policy: none published\n  key_prefixes: none\n  expiry: >-\n    The API User ID and Secret do not expire and there is no documented rotation or revocation\n    procedure. Only the derived access token is short-lived (3600s).\n  scoped_keys: false\n  ip_allowlisting: false\n  note: >-\n    There is no way to issue a restricted credential — no read-only key, no per-integration key,\n    no IP binding. A single compromised API secret grants the full account surface, including\n    the ability to send email from every connected sender mailbox.\n\ntrial_access:\n  note: >-\n    Snov.io states in its API reference that free-plan users must \"request test access by\n    booking a personal demo\". The REST API is a paid-tier feature; the MCP server, by contrast,\n    is documented as available on all plans including the free Trial.\n\nx-evidence:\n  - fetched: '2026-08-13'\n    url: https://snov.io/api\n    http_status: 200\n  - fetched: '2026-08-13'\n    url: https://mcp.snov.io/.well-known/oauth-protected-resource\n\
  \    http_status: 200\n  - fetched: '2026-08-13'\n    url: https://app.snov.io/.well-known/oauth-authorization-server\n    http_status: 200\n  - fetched: '2026-08-13'\n    url: https://mcp.snov.io/mcp\n    http_status: 401\n    detail: 'www-authenticate: Bearer resource_metadata=\"...\", scope=\"mcp\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/authentication/snov-io-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Sales Automation
- Email Finder
- Email Verification
- Lead Generation
- Drip Campaigns
- CRM
- LinkedIn Automation
- Prospect Management
- Data Enrichment
- Cold Email
---
