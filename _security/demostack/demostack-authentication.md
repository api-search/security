---
api_key_in: []
auth_types:
- oauth2
description: 'Demostack publishes no REST API reference and no OpenAPI, so there are no securitySchemes to derive from. The authentication model recorded here was established by probing the surfaces Demostack actually exposes: the OAuth 2.1 authorization server that fronts the Demostack MCP server, and the OAuth 2.0 authorization-code flows documented for the CRM integrations. The user-facing platform itself authenticates with SSO.'
kind: authentication
layout: security
method: probed
name: Demostack Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Demostack secures its APIs with oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Demostack
provider_slug: demostack
scheme_count: 4
schemes:
- client_id_metadata_document_supported: true
  description: OAuth 2.1 authorization server protecting https://mcp.demostack.com/mcp. Supports RFC 7591 dynamic client registration, so an MCP client registers itself and completes the authorization code + PKCE flow with no pre-provisioned credential.
  failure_response:
    body_field: error
    http_status: 401
    value: invalid_token
    www_authenticate: Bearer error="invalid_token", error_description="...", resource_metadata="https://mcp.demostack.com/.well-known/oauth-protected-resource/mcp"
  flows:
  - authorizationUrl: https://mcp.demostack.com/authorize
    codeChallengeMethods:
    - S256
    flow: authorizationCode
    issuer: https://mcp.demostack.com/
    registrationUrl: https://mcp.demostack.com/register
    revocationUrl: https://mcp.demostack.com/revoke
    scopes:
      email: Email address claim
      offline_access: Refresh token issuance
      openid: OpenID Connect subject identifier
      profile: Basic profile claims
    tokenUrl: https://mcp.demostack.com/token
  name: demostack-mcp-oauth
  source: well-known/demostack-oauth-authorization-server.json
  surface: MCP
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
- description: Demostack connects to a customer's Salesforce org using the OAuth 2.0 authorization code grant. Demostack is the client; Salesforce is the authorization server. Tokens are validated before use and refreshed when expired, and Demostack states they are encrypted at rest.
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    callbackUrl: https://api.demostack.com/integrations/salesforce/callback
    flow: authorizationCode
  name: salesforce-integration-oauth
  source: https://help.demostack.com/migration/articles/demostack-and-salesforce-integration-technical-guide
  surface: CRM integration (outbound)
  type: oauth2
- description: Demostack connects to a customer's HubSpot portal through HubSpot's app-authorization redirect flow; the customer selects an account and grants Demostack the required permissions. No endpoint URLs are published.
  name: hubspot-integration-oauth
  source: https://help.demostack.com/migration/articles/demostacks-hubspot-crm-integration-guide
  surface: CRM integration (outbound)
  type: oauth2
- description: Demostack connects to a customer's Slack workspace through Slack's app-approval flow. The customer names the authentication connection, which Demostack then uses to manage the integration. No endpoint URLs are published.
  name: slack-integration-oauth
  source: https://help.demostack.com/migration/articles/demostack-and-slack-integration
  surface: Notification integration (outbound)
  type: oauth2
slug: demostack-authentication
source_filename: demostack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.demostack.com/.well-known/oauth-authorization-server\ndocs: https://help.demostack.com/migration/articles/demostack-and-salesforce-integration-technical-guide\ndescription: >-\n  Demostack publishes no REST API reference and no OpenAPI, so there are no\n  securitySchemes to derive from. The authentication model recorded here was\n  established by probing the surfaces Demostack actually exposes: the OAuth 2.1\n  authorization server that fronts the Demostack MCP server, and the OAuth 2.0\n  authorization-code flows documented for the CRM integrations. The user-facing\n  platform itself authenticates with SSO.\n\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, refreshToken]\n  api_key_in: []\n  dynamic_client_registration: true\n  pkce: S256\n  bearer_methods: [header]\n  note: >-\n    No API key, basic auth, or static-token scheme is documented anywhere on the\n    Demostack public surface.\n\nschemes:\n\
  \  - name: demostack-mcp-oauth\n    type: oauth2\n    surface: MCP\n    source: well-known/demostack-oauth-authorization-server.json\n    description: >-\n      OAuth 2.1 authorization server protecting https://mcp.demostack.com/mcp.\n      Supports RFC 7591 dynamic client registration, so an MCP client registers\n      itself and completes the authorization code + PKCE flow with no\n      pre-provisioned credential.\n    flows:\n      - flow: authorizationCode\n        issuer: https://mcp.demostack.com/\n        authorizationUrl: https://mcp.demostack.com/authorize\n        tokenUrl: https://mcp.demostack.com/token\n        registrationUrl: https://mcp.demostack.com/register\n        revocationUrl: https://mcp.demostack.com/revoke\n        codeChallengeMethods: [S256]\n        scopes:\n          openid: OpenID Connect subject identifier\n          profile: Basic profile claims\n          email: Email address claim\n          offline_access: Refresh token issuance\n    token_endpoint_auth_methods:\
  \ [client_secret_post, client_secret_basic]\n    client_id_metadata_document_supported: true\n    failure_response:\n      http_status: 401\n      body_field: error\n      value: invalid_token\n      www_authenticate: >-\n        Bearer error=\"invalid_token\", error_description=\"...\",\n        resource_metadata=\"https://mcp.demostack.com/.well-known/oauth-protected-resource/mcp\"\n\n  - name: salesforce-integration-oauth\n    type: oauth2\n    surface: CRM integration (outbound)\n    source: https://help.demostack.com/migration/articles/demostack-and-salesforce-integration-technical-guide\n    description: >-\n      Demostack connects to a customer's Salesforce org using the OAuth 2.0\n      authorization code grant. Demostack is the client; Salesforce is the\n      authorization server. Tokens are validated before use and refreshed when\n      expired, and Demostack states they are encrypted at rest.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n\
  \        callbackUrl: https://api.demostack.com/integrations/salesforce/callback\n\n  - name: hubspot-integration-oauth\n    type: oauth2\n    surface: CRM integration (outbound)\n    source: https://help.demostack.com/migration/articles/demostacks-hubspot-crm-integration-guide\n    description: >-\n      Demostack connects to a customer's HubSpot portal through HubSpot's\n      app-authorization redirect flow; the customer selects an account and\n      grants Demostack the required permissions. No endpoint URLs are published.\n\n  - name: slack-integration-oauth\n    type: oauth2\n    surface: Notification integration (outbound)\n    source: https://help.demostack.com/migration/articles/demostack-and-slack-integration\n    description: >-\n      Demostack connects to a customer's Slack workspace through Slack's\n      app-approval flow. The customer names the authentication connection, which\n      Demostack then uses to manage the integration. No endpoint URLs are\n      published.\n\
  \nplatform_authentication:\n  sso: true\n  source: https://www.demostack.com/pricing\n  note: >-\n    Demostack states \"SOC2 compliance, RBAC, and SSO are built into the core\" on\n    its pricing page. This is end-user platform authentication, not an API\n    credential.\n\ngaps:\n  - No public API reference, so no per-operation security requirements exist.\n  - No API key issuance or rotation documentation is published.\n  - >-\n    No /.well-known/openid-configuration is served on any Demostack host; the\n    MCP authorization server advertises openid and profile scopes but publishes\n    only RFC 8414 metadata, not OIDC discovery metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demostack/refs/heads/main/authentication/demostack-authentication.yml
summary_line: oauth2 · 4 schemes
tags:
- Sales Demo
- Demo Automation
- Product Simulation
- Webhook
- CRM Integration
- Sales Enablement
- Presales
- Sales Engineering
- Analytics
- Artificial Intelligence
- MCP
---
