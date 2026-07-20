---
api_key_in:
- header
api_specs:
- filename: knak-enterprise-openapi-original.yml
  format: yaml
  label: Knak Enterprise API
  slug: enterprise
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knak/refs/heads/main/openapi/knak-enterprise-openapi-original.yml
- filename: knak-send-openapi-original.yml
  format: yaml
  label: Knak Send Contacts API
  slug: send
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knak/refs/heads/main/openapi/knak-send-openapi-original.yml
- filename: knak-scim-openapi-original.yml
  format: yaml
  label: Knak SCIM API
  slug: scim
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knak/refs/heads/main/openapi/knak-scim-openapi-original.yml
auth_types:
- http
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Knak Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Knak secures its APIs with http, oauth2, and apiKey across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Knak
provider_slug: knak
scheme_count: 6
schemes:
- applies_to: knak:enterprise
  description: All Knak Enterprise API requests are authenticated with a Bearer token.
  format: 'Authorization: Bearer <token>'
  header: Authorization
  name: Enterprise Bearer token
  scheme: bearer
  sources:
  - https://developer.knak.com/api/
  token_acquisition:
  - description: A user generates a non-expiring token through the Enterprise UI. Knak documents this as generally recommended only for testing and development, or where the OAuth2 flow is not applicable.
    expires: false
    method: api_key
    setup_docs: https://developer.knak.com/api-essentials/api-user-setup/
    setup_notes: Requires an API role with the "Can Manage API Tokens" permission, assigned to a dedicated API user.
    url: https://enterprise.knak.io/account/api-access
  - description: The method Knak recommends for allowing an application access to a customer's Knak data.
    method: oauth2
    url: https://enterprise.knak.io/account/oauth-applications
  type: http
- applies_to: knak:enterprise
  flows:
  - authorizationUrl: https://enterprise.knak.io/oauth/authorize
    csrf: state parameter supported
    flow: authorizationCode
    refresh: refresh_token issued alongside access_token
    response_types:
    - code
    tokenUrl: https://enterprise.knak.io/oauth/token
  name: Knak Enterprise OAuth2
  sources:
  - https://developer.knak.com/api/
  type: oauth2
- applies_to: mcp
  flows:
  - authorizationUrl: https://enterprise.knak.io/oauth/authorize
    dynamic_client_registration: true
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://enterprise.knak.io/oauth/register
    scopes:
    - mcp:use
    tokenUrl: https://enterprise.knak.io/oauth/token
  name: Knak MCP OAuth 2.1
  sources:
  - https://enterprise.knak.io/.well-known/oauth-authorization-server
  type: oauth2
- applies_to: knak:send
  bearerFormat: JWT
  description: A bearer token generated through the Enterprise API Access menu.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/knak-send-openapi-original.yml
  type: http
- applies_to: knak:scim
  description: SCIM 2.0 provisioning requests from the customer's identity provider are authenticated with a bearer token issued in Knak Enterprise.
  name: SCIM Bearer token
  scheme: bearer
  sources:
  - https://developer.knak.com/api/scim/
  type: http
- applies_to: customer-implemented integration contracts
  description: The security header name and value is specified in the Integration Configuration stage in Knak. Used when Knak calls a customer-implemented Custom Validator, Custom DAM or Custom Sync Location endpoint.
  in: header
  name: customSecurityHeader
  parameter: <security-header-name>
  sources:
  - openapi/knak-custom-validator-openapi-original.yml
  type: apiKey
slug: knak-authentication
source_filename: knak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/knak-send-openapi-original.yml, openapi/knak-custom-validator-openapi-original.yml\ndocs: https://developer.knak.com/api/\nsummary:\n  types:\n  - http\n  - oauth2\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  primary: Bearer token in the Authorization header, obtained either as a non-expiring\n    API key or through the OAuth 2.0 authorization code flow.\nschemes:\n- name: Enterprise Bearer token\n  type: http\n  scheme: bearer\n  applies_to: knak:enterprise\n  header: Authorization\n  format: 'Authorization: Bearer <token>'\n  description: All Knak Enterprise API requests are authenticated with a Bearer token.\n  sources:\n  - https://developer.knak.com/api/\n  token_acquisition:\n  - method: api_key\n    description: A user generates a non-expiring token through the Enterprise UI. Knak\n      documents this as generally recommended only for testing and development, or where\n \
  \     the OAuth2 flow is not applicable.\n    url: https://enterprise.knak.io/account/api-access\n    expires: false\n    setup_docs: https://developer.knak.com/api-essentials/api-user-setup/\n    setup_notes: Requires an API role with the \"Can Manage API Tokens\" permission, assigned\n      to a dedicated API user.\n  - method: oauth2\n    description: The method Knak recommends for allowing an application access to a\n      customer's Knak data.\n    url: https://enterprise.knak.io/account/oauth-applications\n- name: Knak Enterprise OAuth2\n  type: oauth2\n  applies_to: knak:enterprise\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://enterprise.knak.io/oauth/authorize\n    tokenUrl: https://enterprise.knak.io/oauth/token\n    response_types:\n    - code\n    csrf: state parameter supported\n    refresh: refresh_token issued alongside access_token\n  sources:\n  - https://developer.knak.com/api/\n- name: Knak MCP OAuth 2.1\n  type: oauth2\n  applies_to: mcp\n  flows:\n\
  \  - flow: authorizationCode\n    pkce: S256\n    dynamic_client_registration: true\n    authorizationUrl: https://enterprise.knak.io/oauth/authorize\n    tokenUrl: https://enterprise.knak.io/oauth/token\n    registrationUrl: https://enterprise.knak.io/oauth/register\n    scopes:\n    - mcp:use\n  sources:\n  - https://enterprise.knak.io/.well-known/oauth-authorization-server\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: knak:send\n  description: A bearer token generated through the Enterprise API Access menu.\n  sources:\n  - openapi/knak-send-openapi-original.yml\n- name: SCIM Bearer token\n  type: http\n  scheme: bearer\n  applies_to: knak:scim\n  description: SCIM 2.0 provisioning requests from the customer's identity provider are\n    authenticated with a bearer token issued in Knak Enterprise.\n  sources:\n  - https://developer.knak.com/api/scim/\n- name: customSecurityHeader\n  type: apiKey\n  in: header\n  parameter: <security-header-name>\n\
  \  applies_to: customer-implemented integration contracts\n  description: The security header name and value is specified in the Integration\n    Configuration stage in Knak. Used when Knak calls a customer-implemented Custom\n    Validator, Custom DAM or Custom Sync Location endpoint.\n  sources:\n  - openapi/knak-custom-validator-openapi-original.yml\nwebhook_authentication:\n  method: hmac-sha256\n  header: knak-signature\n  description: Webhook payloads are signed with a SHA-256 HMAC using a secret generated in\n    Knak. Verify by computing the HMAC of the raw request body and comparing it to the\n    knak-signature header.\n  secret_source: https://enterprise.knak.io/account/webhooks\n  source: openapi/knak-enterprise-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knak/refs/heads/main/authentication/knak-authentication.yml
summary_line: http/oauth2/apiKey · 6 schemes
tags:
- Company
- Email Marketing
- Marketing Automation
- Landing Pages
- Content Creation
- Marketing Operations
- Campaign Management
- No-Code
- SCIM
- Webhooks
---
