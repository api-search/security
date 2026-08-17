---
api_key_in:
- header
api_specs:
- filename: leadiq-graphql-api-openapi.yml
  format: yaml
  label: LeadIQ GraphQL API
  slug: leadiq-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadiq/refs/heads/main/openapi/leadiq-graphql-api-openapi.yml
- filename: leadiq-prospector-api-openapi.yml
  format: yaml
  label: LeadIQ Prospector REST API
  slug: leadiq-prospector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadiq/refs/heads/main/openapi/leadiq-prospector-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Leadiq Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: LeadIQ secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: LeadIQ
provider_slug: leadiq
scheme_count: 4
schemes:
- description: 'The Secret Base64 key issued in Settings -> API is sent verbatim as the Basic credential — it is already the base64 payload, so it is NOT base64-encoded again. Every request is a POST with Content-Type: application/json.'
  header: 'Authorization: Basic <your-secret-base64-api-key>'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/leadiq-graphql-api-openapi.yml
  - https://leadiqhelp.zendesk.com/hc/en-us/articles/29375289152795-LeadIQ-Public-API-Guide
  surface: GraphQL Data API (https://api.leadiq.com/graphql)
  type: http
- description: '"Send your LeadIQ API key as the X-API-Key header value — no prefix, no encoding." The value is the DECODED form of the Secret Base64 key; LeadIQ''s own bash samples run `printf ''%s'' "$LEADIQ_API_KEY" | base64 -d` to produce it.'
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/leadiq-prospector-api-openapi.yml
  - https://leadiqhelp.zendesk.com/hc/en-us/articles/29375289152795-LeadIQ-Public-API-Guide
  surface: Prospector REST API (https://prospector.leadiq.com)
  type: apiKey
- bearerFormat: JWT
  description: Alternative to the API key on the Prospector REST API — "OAuth2 access token (JWT) issued for an audience accepted by this service." Declared as a second top-level security option in the published OpenAPI. LeadIQ does not document how a caller obtains this token outside the MCP flow.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/leadiq-prospector-api-openapi.yml
  surface: Prospector REST API (https://prospector.leadiq.com)
  type: http
- artifact: scopes/leadiq-scopes.yml
  authorization_server: https://leadiq-mcp-prod.us.auth0.com/
  description: OAuth 2.0 with dynamic client registration — no client id or secret to configure. The user signs in with their LeadIQ email/password or Google login and the token carries their own account permissions and credit balance. Discovered from the RFC 9728 protected-resource document, not from a spec.
  flows:
  - authorizationUrl: https://leadiq-mcp-prod.us.auth0.com/authorize
    flow: authorizationCode
    scopes:
    - leadiq:api
    - offline_access
    tokenUrl: https://leadiq-mcp-prod.us.auth0.com/oauth/token
  name: MCPOAuth2
  sources:
  - https://mcp.leadiq.com/.well-known/oauth-protected-resource
  - https://developer.leadiq.com/
  surface: MCP connector (https://mcp.leadiq.com/mcp)
  type: oauth2
slug: leadiq-authentication
source_filename: leadiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/leadiq-graphql-api-openapi.yml, openapi/leadiq-prospector-api-openapi.yml\ndocs: https://leadiqhelp.zendesk.com/hc/en-us/articles/29375289152795-LeadIQ-Public-API-Guide\ndocs_additional:\n- https://developer.leadiq.com/\n- https://github.com/leadiq/api-samples\n- https://mcp.leadiq.com/.well-known/oauth-protected-resource\nkey_issuance: LeadIQ app -> Settings -> API. LeadIQ calls it the \"Secret Base64\" key; it can be rotated from the same page.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  note: >-\n    Three surfaces, three different credentials derived from ONE issued key. The\n    GraphQL Data API takes the Secret Base64 key verbatim as an HTTP Basic credential;\n    the Prospector REST API takes the SAME key base64-DECODED, in an X-API-Key header;\n    the MCP connector ignores API keys entirely and uses OAuth 2.0 against LeadIQ's\n\
  \    Auth0 tenant with dynamic client registration. LeadIQ's own bash sample pipes the\n    key through `base64 -d` when crossing from the GraphQL scripts to the REST ones,\n    which is the clearest published statement of that relationship.\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  surface: GraphQL Data API (https://api.leadiq.com/graphql)\n  header: 'Authorization: Basic <your-secret-base64-api-key>'\n  description: >-\n    The Secret Base64 key issued in Settings -> API is sent verbatim as the Basic\n    credential — it is already the base64 payload, so it is NOT base64-encoded again.\n    Every request is a POST with Content-Type: application/json.\n  sources:\n  - openapi/leadiq-graphql-api-openapi.yml\n  - https://leadiqhelp.zendesk.com/hc/en-us/articles/29375289152795-LeadIQ-Public-API-Guide\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  surface: Prospector REST API (https://prospector.leadiq.com)\n  description: >-\n    \"Send\
  \ your LeadIQ API key as the X-API-Key header value — no prefix, no encoding.\"\n    The value is the DECODED form of the Secret Base64 key; LeadIQ's own bash samples\n    run `printf '%s' \"$LEADIQ_API_KEY\" | base64 -d` to produce it.\n  sources:\n  - openapi/leadiq-prospector-api-openapi.yml\n  - https://leadiqhelp.zendesk.com/hc/en-us/articles/29375289152795-LeadIQ-Public-API-Guide\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  surface: Prospector REST API (https://prospector.leadiq.com)\n  description: >-\n    Alternative to the API key on the Prospector REST API — \"OAuth2 access token (JWT)\n    issued for an audience accepted by this service.\" Declared as a second top-level\n    security option in the published OpenAPI. LeadIQ does not document how a caller\n    obtains this token outside the MCP flow.\n  sources:\n  - openapi/leadiq-prospector-api-openapi.yml\n- name: MCPOAuth2\n  type: oauth2\n  surface: MCP connector (https://mcp.leadiq.com/mcp)\n\
  \  description: >-\n    OAuth 2.0 with dynamic client registration — no client id or secret to configure.\n    The user signs in with their LeadIQ email/password or Google login and the token\n    carries their own account permissions and credit balance. Discovered from the RFC\n    9728 protected-resource document, not from a spec.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://leadiq-mcp-prod.us.auth0.com/authorize\n    tokenUrl: https://leadiq-mcp-prod.us.auth0.com/oauth/token\n    scopes: [leadiq:api, offline_access]\n  authorization_server: https://leadiq-mcp-prod.us.auth0.com/\n  artifact: scopes/leadiq-scopes.yml\n  sources:\n  - https://mcp.leadiq.com/.well-known/oauth-protected-resource\n  - https://developer.leadiq.com/\nfailure_modes:\n- {status: 401, meaning: Invalid or missing API key}\n- {status: 402, meaning: Insufficient credits}\nnotes:\n- Never commit the key; rotate it from Settings -> API if compromised (provider guidance).\n- Enterprise SSO orgs\
  \ signing into the MCP connector should enter their email address directly rather than using \"Sign in with Google\", which errors when the org's Google domain is linked to LeadIQ.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadiq/refs/heads/main/authentication/leadiq-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Sales Intelligence
- B2B Data
- Contact Data
- Lead Generation
- Prospecting
- CRM Enrichment
- Sales Engagement
- GraphQL
- Model Context Protocol
- Revenue Operations
- Go To Market
---
