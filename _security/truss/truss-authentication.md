---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Truss API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Truss Authentication
name_suffix: Authentication
oauth_flows: []
overview: Truss declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Truss
provider_slug: truss
scheme_count: 3
schemes:
- authorize_url: https://app.trusspayments.com/oauth/authorize
  evidence: Truss API endpoints use **Bearer token** authentication. All API requests require a valid JWT access token in the `Authorization` header.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Obtain OAuth credentials (client_id, client_secret, redirect_uri) from Truss, then perform the OAuth 2.0 Authorization Code flow to receive an access token.
  location: header
  name: Bearer JWT
  scopes:
  - offline_access
  - payment_intent.inbound:read
  - payment_intent.inbound:write
  - payment_intent.outbound:read
  - payment_intent.outbound:write
  - contacts:read
  - contacts:write
  - transactions:read
  - wallets:read
  - company:read
  - accounts:read
  type: http-bearer
- authorize_url: https://app.trusspayments.com/oauth/authorize
  evidence: Access tokens are obtained through the OAuth 2.0 Authorization Code flow on the Truss Auth server.
  flows:
  - authorization_code
  how_to_obtain: Contact Truss to obtain client_id, client_secret, and approved redirect_uri, then follow the OAuth Integration Guide to perform the Authorization Code flow.
  name: OAuth 2.0 Authorization Code
  scopes:
  - offline_access
  - payment_intent.inbound:read
  - payment_intent.inbound:write
  - payment_intent.outbound:read
  - payment_intent.outbound:write
  - contacts:read
  - contacts:write
  - transactions:read
  - wallets:read
  - company:read
  - accounts:read
  type: oauth2
- evidence: Use the **Base Auth URL** to complete the authorization code exchange and to refresh tokens.
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: POST to the token endpoint with grant_type=authorization_code (or refresh_token) along with client_id, client_secret, and other required parameters.
  name: OAuth 2.0 Token Endpoint
  token_url: https://auth.foundation.trusspayments.com/v1/oauth2/token
  type: oauth2
slug: truss-authentication
source_filename: truss-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.trusspayments.com/guides/authentication/overview/index.md
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.trusspayments.com/guides/authentication/overview/index.md\nsources:\n- https://docs.trusspayments.com/guides/authentication/overview/index.md\n- https://docs.trusspayments.com/guides/authentication/oauth-integration-guide/index.md\n- https://docs.trusspayments.com/guides/authentication/scopes/index.md\n- https://docs.trusspayments.com/guides/authentication/overview\ndescription: Authentication schemes for Truss API\nschemes:\n- type: http-bearer\n  name: Bearer JWT\n  evidence: Truss API endpoints use **Bearer token** authentication. All API requests require a valid JWT access token in the `Authorization`\n    header.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://app.trusspayments.com/oauth/authorize\n  scopes:\n  - offline_access\n  - payment_intent.inbound:read\n  - payment_intent.inbound:write\n  - payment_intent.outbound:read\n\
  \  - payment_intent.outbound:write\n  - contacts:read\n  - contacts:write\n  - transactions:read\n  - wallets:read\n  - company:read\n  - accounts:read\n  how_to_obtain: Obtain OAuth credentials (client_id, client_secret, redirect_uri) from Truss, then perform the OAuth 2.0 Authorization Code flow\n    to receive an access token.\n- type: oauth2\n  name: OAuth 2.0 Authorization Code\n  evidence: Access tokens are obtained through the OAuth 2.0 Authorization Code flow on the Truss Auth server.\n  flows:\n  - authorization_code\n  authorize_url: https://app.trusspayments.com/oauth/authorize\n  scopes:\n  - offline_access\n  - payment_intent.inbound:read\n  - payment_intent.inbound:write\n  - payment_intent.outbound:read\n  - payment_intent.outbound:write\n  - contacts:read\n  - contacts:write\n  - transactions:read\n  - wallets:read\n  - company:read\n  - accounts:read\n  how_to_obtain: Contact Truss to obtain client_id, client_secret, and approved redirect_uri, then follow the OAuth Integration\
  \ Guide to perform\n    the Authorization Code flow.\n- type: oauth2\n  name: OAuth 2.0 Token Endpoint\n  evidence: Use the **Base Auth URL** to complete the authorization code exchange and to refresh tokens.\n  flows:\n  - authorization_code\n  - refresh_token\n  token_url: https://auth.foundation.trusspayments.com/v1/oauth2/token\n  how_to_obtain: POST to the token endpoint with grant_type=authorization_code (or refresh_token) along with client_id, client_secret, and other\n    required parameters.\ndocs: https://docs.trusspayments.com/guides/authentication/overview/index.md\n"
source_yaml_url: https://artifacts.apis.io/truss/authentication/truss-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Banking
- Construction
- Payments
- FinTech
---
