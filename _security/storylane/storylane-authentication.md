---
api_key_in: []
api_specs:
- filename: storylane-connect
  format: yaml
  label: Storylane External API
  slug: storylane-external-api
  spec_type: Postman
  url: https://www.postman.com/team-storylane/storylane-public/collection/2zkg7jc/storylane-connect
auth_types: []
description: 'Storylane runs three distinct authentication models across three distinct surfaces, and they do not share credentials. The remote MCP server uses full OAuth 2.0 with dynamic client registration and PKCE. The External REST API uses a manually issued, non-recoverable Bearer token paired with a workspace identifier. Webhooks are unauthenticated inbound POSTs verified by an HMAC-SHA256 signature header. Workspace login itself is SAML/OIDC SSO brokered through WorkOS, with SCIM provisioning.

  '
kind: authentication
layout: security
method: searched
name: Storylane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Storylane declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Storylane
provider_slug: storylane
scheme_count: 5
schemes:
- authorization_endpoint: https://identity.storylane.io/oauth/authorize
  code_challenge_methods_supported:
  - S256
  dynamic_client_registration: true
  dynamic_client_registration_spec: RFC 7591
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  http_status: 401
  id: mcp_oauth2
  issuer: https://identity.storylane.io
  metadata_document: https://identity.storylane.io/.well-known/oauth-authorization-server
  metadata_spec: RFC 8414
  note: 'Public-client friendly: token_endpoint_auth_methods_supported includes "none" and PKCE S256 is offered, which is exactly the shape an MCP desktop client needs. Combined with an open registration_endpoint, an MCP client can register and authorize without any human at Storylane touching it — the opposite of how the REST API is provisioned.

    '
  pkce: true
  registration_endpoint: https://identity.storylane.io/oauth/register
  response_types_supported:
  - code
  scopes:
  - mcp
  - demos_read
  - demos_write
  - analytics_read
  scopes_detail: scopes/storylane-scopes.yml
  self_serve: true
  surface: Storylane MCP (https://identity.storylane.io/mcp)
  token_endpoint: https://identity.storylane.io/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  type: oauth2
  verified: probed
  www_authenticate: Bearer realm="Storylane MCP"
- additional_credential:
    description: Unique identifier for the customer workspace, issued alongside the token.
    name: workspace_id
  expiry_documented: false
  format: 'Authorization: Bearer <access_token>'
  header: Authorization
  id: external_api_bearer
  in: header
  plan_gate: Enterprise plan only.
  provisioning: 'Manual. Customers email support@storylane.io to request a workspace_id and access_token; credentials are issued only after approval.

    '
  recoverable: false
  recovery_note: 'Storylane states it does not store the access_token server-side and cannot re-issue or retrieve a lost one — the customer must store it securely or request a new credential.

    '
  rotation_documented: false
  scheme: bearer
  scopes: none
  self_serve: false
  surface: Storylane External REST API (https://api.storylane.io)
  type: http
- algorithm: HMAC-SHA256
  direction: inbound-to-customer
  encoding: base64
  header: x-storylane-signature
  id: webhook_hmac
  note: 'Storylane publishes verified reference implementations in Node.js/Express, Ruby and Python/Flask, and its Ruby and Python examples use constant-time comparison (Rack::Utils.secure_compare, hmac.compare_digest). The Node example uses a plain === comparison, which is timing-unsafe — worth flagging to any integrator copying it verbatim.

    '
  replay_protection_documented: false
  secret_location: Storylane dashboard, Settings > Integrations > Webhook
  secret_name: Webhook Verification Secret
  signed_payload: raw request body (unparsed)
  surface: Storylane outbound webhooks (customer-hosted receiver)
  timestamp_in_signature: false
  type: signature
- broker: WorkOS
  id: workspace_sso
  identity_providers_documented:
  - Okta SAML
  - OneLogin SAML
  - Auth0
  - Azure AD SAML
  - Google SAML
  - Microsoft AD FS SAML
  - ADP OpenID Connect
  - Generic OpenID Connect
  - CAS SAML
  - ClassLink
  - Cloudflare SAML
  - CyberArk SAML
  - Duo SAML
  - Generic SAML
  - JumpCloud SAML
  - Keycloak SAML
  - miniOrange SAML
  - Oracle SAML
  - PingFederate SAML
  - PingOne SAML
  - Salesforce SAML
  - SimpleSAMLphp
  - VMware SAML
  plan_gate: Premium plan and above (Single Sign-on is listed on Premium).
  protocols:
  - SAML 2.0
  - OpenID Connect
  - Google OAuth
  - Microsoft OAuth
  provisioning:
    scim: true
    scim_note: 'SCIM automated user provisioning is supported but must be enabled by Storylane support; it is not self-serve in the dashboard.

      '
    scim_spec: SCIM 2.0
  surface: Storylane application login (https://app.storylane.io)
  type: openIdConnect / saml
- http_status: 200
  id: anonymous_oembed
  note: 'The oEmbed metadata endpoint accepts a public demo share URL and returns an oEmbed 1.0 rich response with no credential of any kind. It is the only Storylane API endpoint reachable anonymously.

    '
  surface: https://api.storylane.io/oembed/meta
  type: none
  verified: probed
slug: storylane-authentication
source_filename: storylane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >\n  https://docs.storylane.io/integrations/integrations-and-data-flow/external-api,\n  https://docs.storylane.io/integrations/integrations-and-data-flow/mcp,\n  https://docs.storylane.io/integrations/integrations-and-data-flow/webhooks,\n  https://docs.storylane.io/trust-and-security/sso, and live probes of\n  https://identity.storylane.io/.well-known/oauth-authorization-server\ndescription: >\n  Storylane runs three distinct authentication models across three distinct\n  surfaces, and they do not share credentials. The remote MCP server uses full\n  OAuth 2.0 with dynamic client registration and PKCE. The External REST API uses\n  a manually issued, non-recoverable Bearer token paired with a workspace\n  identifier. Webhooks are unauthenticated inbound POSTs verified by an\n  HMAC-SHA256 signature header. Workspace login itself is SAML/OIDC SSO brokered\n  through WorkOS, with SCIM provisioning.\nschemes:\n  - id: mcp_oauth2\n\
  \    surface: Storylane MCP (https://identity.storylane.io/mcp)\n    type: oauth2\n    verified: probed\n    http_status: 401\n    www_authenticate: Bearer realm=\"Storylane MCP\"\n    issuer: https://identity.storylane.io\n    metadata_document: https://identity.storylane.io/.well-known/oauth-authorization-server\n    metadata_spec: RFC 8414\n    authorization_endpoint: https://identity.storylane.io/oauth/authorize\n    token_endpoint: https://identity.storylane.io/oauth/token\n    registration_endpoint: https://identity.storylane.io/oauth/register\n    dynamic_client_registration: true\n    dynamic_client_registration_spec: RFC 7591\n    pkce: true\n    code_challenge_methods_supported:\n      - S256\n    response_types_supported:\n      - code\n    grant_types_supported:\n      - authorization_code\n      - client_credentials\n      - refresh_token\n    token_endpoint_auth_methods_supported:\n      - none\n      - client_secret_post\n    scopes:\n      - mcp\n      - demos_read\n  \
  \    - demos_write\n      - analytics_read\n    scopes_detail: scopes/storylane-scopes.yml\n    self_serve: true\n    note: >\n      Public-client friendly: token_endpoint_auth_methods_supported includes\n      \"none\" and PKCE S256 is offered, which is exactly the shape an MCP desktop\n      client needs. Combined with an open registration_endpoint, an MCP client\n      can register and authorize without any human at Storylane touching it —\n      the opposite of how the REST API is provisioned.\n  - id: external_api_bearer\n    surface: Storylane External REST API (https://api.storylane.io)\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: \"Authorization: Bearer <access_token>\"\n    additional_credential:\n      name: workspace_id\n      description: Unique identifier for the customer workspace, issued alongside the token.\n    self_serve: false\n    provisioning: >\n      Manual. Customers email support@storylane.io to request a workspace_id\
  \ and\n      access_token; credentials are issued only after approval.\n    plan_gate: Enterprise plan only.\n    recoverable: false\n    recovery_note: >\n      Storylane states it does not store the access_token server-side and cannot\n      re-issue or retrieve a lost one — the customer must store it securely or\n      request a new credential.\n    rotation_documented: false\n    expiry_documented: false\n    scopes: none\n  - id: webhook_hmac\n    surface: Storylane outbound webhooks (customer-hosted receiver)\n    type: signature\n    direction: inbound-to-customer\n    header: x-storylane-signature\n    algorithm: HMAC-SHA256\n    encoding: base64\n    signed_payload: raw request body (unparsed)\n    secret_name: Webhook Verification Secret\n    secret_location: Storylane dashboard, Settings > Integrations > Webhook\n    timestamp_in_signature: false\n    replay_protection_documented: false\n    note: >\n      Storylane publishes verified reference implementations in Node.js/Express,\n\
  \      Ruby and Python/Flask, and its Ruby and Python examples use constant-time\n      comparison (Rack::Utils.secure_compare, hmac.compare_digest). The Node\n      example uses a plain === comparison, which is timing-unsafe — worth flagging\n      to any integrator copying it verbatim.\n  - id: workspace_sso\n    surface: Storylane application login (https://app.storylane.io)\n    type: openIdConnect / saml\n    broker: WorkOS\n    protocols:\n      - SAML 2.0\n      - OpenID Connect\n      - Google OAuth\n      - Microsoft OAuth\n    identity_providers_documented:\n      - Okta SAML\n      - OneLogin SAML\n      - Auth0\n      - Azure AD SAML\n      - Google SAML\n      - Microsoft AD FS SAML\n      - ADP OpenID Connect\n      - Generic OpenID Connect\n      - CAS SAML\n      - ClassLink\n      - Cloudflare SAML\n      - CyberArk SAML\n      - Duo SAML\n      - Generic SAML\n      - JumpCloud SAML\n      - Keycloak SAML\n      - miniOrange SAML\n      - Oracle SAML\n      - PingFederate\
  \ SAML\n      - PingOne SAML\n      - Salesforce SAML\n      - SimpleSAMLphp\n      - VMware SAML\n    plan_gate: Premium plan and above (Single Sign-on is listed on Premium).\n    provisioning:\n      scim: true\n      scim_spec: SCIM 2.0\n      scim_note: >\n        SCIM automated user provisioning is supported but must be enabled by\n        Storylane support; it is not self-serve in the dashboard.\n  - id: anonymous_oembed\n    surface: https://api.storylane.io/oembed/meta\n    type: none\n    verified: probed\n    http_status: 200\n    note: >\n      The oEmbed metadata endpoint accepts a public demo share URL and returns an\n      oEmbed 1.0 rich response with no credential of any kind. It is the only\n      Storylane API endpoint reachable anonymously.\ngaps:\n  - No /.well-known/openid-configuration is served on any Storylane host — only the OAuth 2.0 authorization server metadata.\n  - No /.well-known/oauth-protected-resource is served, so an MCP client cannot discover the resource\
  \ server metadata from the endpoint itself; it must be given the issuer.\n  - The External REST API publishes no token rotation, expiry or revocation policy.\n  - No mutual TLS, no request signing and no IP allowlist are documented for the REST API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storylane/refs/heads/main/authentication/storylane-authentication.yml
summary_line: 5 schemes
tags:
- Interactive Demos
- Product Walkthroughs
- Sales Enablement
- Marketing
- Demo Analytics
- Demo Automation
- Buyer Hub
- Sales
- MCP
- Agent Tools
- Webhooks
- Embeds
- oEmbed
- Demo Automation Platform
---
