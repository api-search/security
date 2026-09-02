---
api_key_in: []
auth_types: []
description: '6sense runs two distinct authentication surfaces. The REST APIs (api.6sense.com, epsilon.6sense.com, scribe.6sense.com) use a customer-issued API token in an `Authorization: Token <api_token>` header — note the `Token` scheme, not `Bearer`. The MCP server at https://api.6sense.com/mcp is a separate OAuth 2.0 protected resource with per-user authorization, dynamic client registration and the single scope `mcp:use`.'
kind: authentication
layout: security
method: searched
name: 6Sense Insights Authentication
name_suffix: Authentication
oauth_flows: []
overview: 6Sense Insights declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: 6Sense Insights
provider_slug: 6sense-insights
scheme_count: 3
schemes:
- applies_to:
  - Company Identification API
  - Company Firmographics API
  - Lead Scoring API
  - Lead Scoring and Firmographics API
  - People Enrichment API
  - People Search API
  docs: https://api.6sense.com/docs/#get-your-api-token
  example: 'Authorization: Token <api_token>'
  id: api_token
  in: header
  issuance: Self-service in the 6sense Platform under Settings > API Token management > Generate New API token, scoped by API group. Tokens can only be generated for API groups covered by the customer's purchased credit type. Segments API tokens must be requested from 6sense support.
  key_format: 40-character randomly generated alphanumeric string
  name: Authorization
  provider_guidance:
  - Name each token after the integration it is used by.
  - Do not reuse one token across multiple integrations.
  - Rotate API tokens every 90 days.
  - Deactivate unused tokens and delete tokens no longer planned for use.
  - Enrichment API tokens must never be exposed on a public domain — those APIs are designed for server-to-server calls only.
  - Token settings (Score and Segments Settings) are secure by default and return no detailed information until explicitly widened.
  scheme_prefix: 'Token '
  type: apiKey
- description: Additional header partners must send for customer data identification. Format `<partner_name>-<customer_name>-<customer_api_token>` when calling on behalf of a customer, or `<partner_name>-<partner_api_token>` when calling with the partner's own token.
  docs: https://api.6sense.com/docs/
  id: partner_custom_id
  in: header
  name: X-6s-CustomID
  required: false
  type: apiKey
- applies_to:
  - 6sense MCP server (https://api.6sense.com/mcp)
  code_challenge_methods_supported:
  - S256
  detail: well-known/6sense-insights-oauth-authorization-server.json
  dpop_supported: true
  dynamic_client_registration: true
  flows:
    authorization_code:
      authorization_url: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/authorize
      scopes:
        mcp:use: Read-only access to 6sense data through the MCP server.
      token_url: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token
    client_credentials:
      token_url: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:openid:params:grant-type:ciba
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:token-exchange
  id: mcp_oauth2
  issuer: https://auth.6sense.com/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN
  jwks_uri: https://auth.6sense.com/P32lusHUPY06hG8MJtqJnKEmq7hJ/.well-known/jwks.json
  per_user_authorization: true
  registration_endpoint: https://auth.6sense.com/v1/mgmt/mcp/client/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/register
  revocation_endpoint: https://auth.6sense.com/oauth2/v1/apps/P32lusHUPY06hG8MJtqJnKEmq7hJ/revoke
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfo_endpoint: https://auth.6sense.com/oauth2/v1/apps/P32lusHUPY06hG8MJtqJnKEmq7hJ/userinfo
slug: 6sense-insights-authentication
source_filename: 6sense-insights-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://api.6sense.com/docs/ (Get your API Token / Headers sections) and\n  https://api.6sense.com/.well-known/oauth-authorization-server (probed live).\ndescription: >-\n  6sense runs two distinct authentication surfaces. The REST APIs\n  (api.6sense.com, epsilon.6sense.com, scribe.6sense.com) use a customer-issued\n  API token in an `Authorization: Token <api_token>` header — note the `Token`\n  scheme, not `Bearer`. The MCP server at https://api.6sense.com/mcp is a\n  separate OAuth 2.0 protected resource with per-user authorization, dynamic\n  client registration and the single scope `mcp:use`.\n\nschemes:\n  - id: api_token\n    type: apiKey\n    in: header\n    name: Authorization\n    scheme_prefix: 'Token '\n    example: 'Authorization: Token <api_token>'\n    applies_to:\n      - Company Identification API\n      - Company Firmographics API\n      - Lead Scoring API\n      - Lead Scoring and Firmographics API\n\
  \      - People Enrichment API\n      - People Search API\n    key_format: 40-character randomly generated alphanumeric string\n    issuance: >-\n      Self-service in the 6sense Platform under Settings > API Token management\n      > Generate New API token, scoped by API group. Tokens can only be\n      generated for API groups covered by the customer's purchased credit type.\n      Segments API tokens must be requested from 6sense support.\n    provider_guidance:\n      - Name each token after the integration it is used by.\n      - Do not reuse one token across multiple integrations.\n      - Rotate API tokens every 90 days.\n      - Deactivate unused tokens and delete tokens no longer planned for use.\n      - >-\n        Enrichment API tokens must never be exposed on a public domain — those\n        APIs are designed for server-to-server calls only.\n      - >-\n        Token settings (Score and Segments Settings) are secure by default and\n        return no detailed information until\
  \ explicitly widened.\n    docs: https://api.6sense.com/docs/#get-your-api-token\n\n  - id: partner_custom_id\n    type: apiKey\n    in: header\n    name: X-6s-CustomID\n    required: false\n    description: >-\n      Additional header partners must send for customer data identification.\n      Format `<partner_name>-<customer_name>-<customer_api_token>` when calling\n      on behalf of a customer, or `<partner_name>-<partner_api_token>` when\n      calling with the partner's own token.\n    docs: https://api.6sense.com/docs/\n\n  - id: mcp_oauth2\n    type: oauth2\n    applies_to:\n      - 6sense MCP server (https://api.6sense.com/mcp)\n    flows:\n      authorization_code:\n        authorization_url: >-\n          https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/authorize\n        token_url: >-\n          https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token\n        scopes:\n\
  \          mcp:use: Read-only access to 6sense data through the MCP server.\n      client_credentials:\n        token_url: >-\n          https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token\n    issuer: >-\n      https://auth.6sense.com/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN\n    jwks_uri: https://auth.6sense.com/P32lusHUPY06hG8MJtqJnKEmq7hJ/.well-known/jwks.json\n    registration_endpoint: >-\n      https://auth.6sense.com/v1/mgmt/mcp/client/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/register\n    revocation_endpoint: https://auth.6sense.com/oauth2/v1/apps/P32lusHUPY06hG8MJtqJnKEmq7hJ/revoke\n    userinfo_endpoint: https://auth.6sense.com/oauth2/v1/apps/P32lusHUPY06hG8MJtqJnKEmq7hJ/userinfo\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n      - client_credentials\n      - urn:openid:params:grant-type:ciba\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n\
  \      - urn:ietf:params:oauth:grant-type:token-exchange\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [none, client_secret_basic, client_secret_post]\n    dpop_supported: true\n    dynamic_client_registration: true\n    per_user_authorization: true\n    detail: well-known/6sense-insights-oauth-authorization-server.json\n\nunauthenticated_surface:\n  - >-\n    The Company Identification API can be invoked client-side through the\n    6sense WebTag without the customer creating an API token; the WebTag carries\n    its own configuration. Direct (non-WebTag) use of that API does require a\n    token.\n\nfailure_response:\n  status: 401\n  body: >-\n    Your API token is invalid or auth token is invalid or missing authorization\n    header.\n  detail: errors/6sense-insights-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6sense-insights/refs/heads/main/authentication/6sense-insights-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Account Based Marketing
- Intent Data
- B2B
- Predictive Analytics
- Revenue
- Sales Intelligence
- Marketing Technology
- Artificial Intelligence
- Data Enrichment
---
