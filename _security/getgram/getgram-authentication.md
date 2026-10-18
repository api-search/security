---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getgram-openapi-generated.yml
  format: yaml
  label: Gram (by Speakeasy) API
  slug: getgram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getgram/refs/heads/main/openapi/_ae-authored/getgram-openapi-generated.yml
auth_types: []
description: Authentication methods described for Gram (by Speakeasy) MCP servers.
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Getgram Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gram (by Speakeasy) declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Gram (by Speakeasy)
provider_slug: getgram
scheme_count: 5
schemes:
- evidence: 'Service Account : every caller shares one identity, sent to the upstream service as the Authorization header. The credential is either Static (a Bearer token, a Basic username and password, or a Manual header value) or OAuth (an access token the platform obtains for itself with the client credentials grant, using a Client Secret or a Signing Client ).'
  header: Authorization
  how_to_obtain: Static bearer token configured in the Service Account settings or obtained via OAuth client credentials grant.
  location: header
  name: Service Account Bearer Token
  type: http-bearer
- evidence: 'Service Account : every caller shares one identity, sent to the upstream service as the Authorization header. The credential is either Static (a Bearer token, a Basic username and password, or a Manual header value) or OAuth (an access token the platform obtains for itself with the client credentials grant, using a Client Secret or a Signing Client ).'
  header: Authorization
  how_to_obtain: Static username and password configured in the Service Account settings.
  location: header
  name: Service Account Basic Auth
  type: http-basic
- evidence: The Authorization Code Flow enables user-interactive OAuth with proper consent screens.
  how_to_obtain: User interacts with provider’s authorization endpoint; client receives code and exchanges for token.
  name: Authorization Code Grant
  type: oauth2
- evidence: The Client Credentials grant is a simpler authentication method. The server exchanges a client ID and secret for access tokens.
  how_to_obtain: Server sends client_id and client_secret to token endpoint to obtain access token.
  name: Client Credentials Grant
  type: oauth2
- evidence: API keys authenticate programmatic access to the platform, such as MCP deployments, tool management, telemetry ingestion, and device‑agent enrollment.
  header: Authorization
  how_to_obtain: Created via Organization settings > API Keys; full token shown once at creation.
  location: header
  name: API Key
  type: apiKey
slug: getgram-authentication
source_filename: getgram-authentication.yml
source_heading: Authentication Profile
source_url: https://www.speakeasy.com/docs/ai-control-plane/mcp-gateway/access
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.speakeasy.com/docs/ai-control-plane/mcp-gateway/access\nsources:\n- https://www.speakeasy.com/docs/ai-control-plane/mcp-gateway/access\n- https://www.speakeasy.com/docs/ai-control-plane/org-admin/api-keys\n- https://www.speakeasy.com/docs/ai-control-plane/guides/oauth-external-server\n- https://www.speakeasy.com/docs/standalone-mcp/setting-up-oauth\ndescription: Authentication methods described for Gram (by Speakeasy) MCP servers.\nschemes:\n- type: http-bearer\n  name: Service Account Bearer Token\n  evidence: 'Service Account : every caller shares one identity, sent to the upstream service as the Authorization header. The credential is either\n    Static (a Bearer token, a Basic username and password, or a Manual header value) or OAuth (an access token the platform obtains for itself\n    with the client credentials grant, using a Client Secret or a Signing Client\
  \ ).'\n  location: header\n  header: Authorization\n  how_to_obtain: Static bearer token configured in the Service Account settings or obtained via OAuth client credentials grant.\n- type: http-basic\n  name: Service Account Basic Auth\n  evidence: 'Service Account : every caller shares one identity, sent to the upstream service as the Authorization header. The credential is either\n    Static (a Bearer token, a Basic username and password, or a Manual header value) or OAuth (an access token the platform obtains for itself\n    with the client credentials grant, using a Client Secret or a Signing Client ).'\n  location: header\n  header: Authorization\n  how_to_obtain: Static username and password configured in the Service Account settings.\n- type: oauth2\n  name: Authorization Code Grant\n  evidence: The Authorization Code Flow enables user-interactive OAuth with proper consent screens.\n  how_to_obtain: User interacts with provider’s authorization endpoint; client receives code and\
  \ exchanges for token.\n- type: oauth2\n  name: Client Credentials Grant\n  evidence: The Client Credentials grant is a simpler authentication method. The server exchanges a client ID and secret for access tokens.\n  how_to_obtain: Server sends client_id and client_secret to token endpoint to obtain access token.\n- type: apiKey\n  name: API Key\n  evidence: API keys authenticate programmatic access to the platform, such as MCP deployments, tool management, telemetry ingestion, and device‑agent\n    enrollment.\n  location: header\n  header: Authorization\n  how_to_obtain: Created via Organization settings > API Keys; full token shown once at creation.\ndocs: https://www.speakeasy.com/docs/ai-control-plane/mcp-gateway/access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getgram/refs/heads/main/authentication/getgram-authentication.yml
summary_line: 5 schemes
tags:
- Company
- AI
- ConversationalAI
- Chatbots
- Platform
---
