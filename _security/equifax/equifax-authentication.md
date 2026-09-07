---
anonymous_access: false
api_key_in: []
auth_types: []
description: Every Equifax API product on the Equifax Developer Portal is protected by OAuth 2.0 using the client_credentials grant. Credentials (Client ID + Client Secret) are issued per application AND per environment when an app is created in the portal and connected to one or more API Products. A bearer Access Token obtained from the environment's token endpoint must accompany every request; Equifax returns HTTP 401 for a missing or invalid token. Production additionally enforces IP allow-listing on top of a valid token — a second control that is configured per application in the portal.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Equifax Authentication
name_suffix: Authentication
oauth_flows: []
overview: Equifax declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Equifax
provider_slug: equifax
scheme_count: 1
schemes:
- credentials_scope: per application, per environment
  flow: clientCredentials
  header: Authorization
  id: oauth2_client_credentials
  in: header
  parameters:
  - client_id
  - client_secret
  - scope
  quote: '"The type of access called ''OAuth 2.0 grant type'' used for Equifax APIs is client credentials - here the username and password are not required. Rather, you obtain the Access Token by providing only the client_id, client_secret, and the scope."'
  scheme: Bearer
  scopes_documented: false
  scopes_note: The docs state the token request carries a `scope`, and the quick-start guide tells integrators to "Expand each API to confirm the appropriate endpoint 'Scope' to use in test mode" — the scope VALUES are per-API-product and are only rendered on the signed-in application page in the developer portal. No public scope reference is published.
  token_endpoint: https://api.equifax.com/v2/oauth/token
  token_endpoint_evidence: An unauthenticated POST of an empty form body (and of grant_type=client_credentials alone) to https://api.equifax.com/v2/oauth/token returned HTTP 400 with {"error":"invalid_request","error_description":"Missing Mandatory Parameters"} on 2026-09-06 — an RFC 6749 error response from a live token endpoint, not the {"efxErrorCode":"404.01"} envelope the same gateway returns for an unrouted path. https://api.sandbox.equifax.com/v2/oauth/token returned the identical body. No credentials were sent and none were obtained.
  token_endpoint_sandbox: https://api.sandbox.equifax.com/v2/oauth/token
  token_endpoint_verified: probed
  type: oauth2
slug: equifax-authentication
source_filename: equifax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://developer.equifax.com/documentation\ndocs: https://developer.equifax.com/documentation\nprovider: Equifax\nproviderId: equifax\ndescription: >-\n  Every Equifax API product on the Equifax Developer Portal is protected by OAuth 2.0\n  using the client_credentials grant. Credentials (Client ID + Client Secret) are issued\n  per application AND per environment when an app is created in the portal and connected\n  to one or more API Products. A bearer Access Token obtained from the environment's\n  token endpoint must accompany every request; Equifax returns HTTP 401 for a missing or\n  invalid token. Production additionally enforces IP allow-listing on top of a valid\n  token — a second control that is configured per application in the portal.\nschemes:\n  - id: oauth2_client_credentials\n    type: oauth2\n    flow: clientCredentials\n    in: header\n    header: Authorization\n    scheme: Bearer\n    token_endpoint: https://api.equifax.com/v2/oauth/token\n\
  \    token_endpoint_sandbox: https://api.sandbox.equifax.com/v2/oauth/token\n    token_endpoint_verified: probed\n    token_endpoint_evidence: >-\n      An unauthenticated POST of an empty form body (and of grant_type=client_credentials\n      alone) to https://api.equifax.com/v2/oauth/token returned HTTP 400 with\n      {\"error\":\"invalid_request\",\"error_description\":\"Missing Mandatory Parameters\"} on\n      2026-09-06 — an RFC 6749 error response from a live token endpoint, not the\n      {\"efxErrorCode\":\"404.01\"} envelope the same gateway returns for an unrouted path.\n      https://api.sandbox.equifax.com/v2/oauth/token returned the identical body. No\n      credentials were sent and none were obtained.\n    parameters:\n      - client_id\n      - client_secret\n      - scope\n    scopes_documented: false\n    scopes_note: >-\n      The docs state the token request carries a `scope`, and the quick-start guide tells\n      integrators to \"Expand each API to confirm the appropriate\
  \ endpoint 'Scope' to use\n      in test mode\" — the scope VALUES are per-API-product and are only rendered on the\n      signed-in application page in the developer portal. No public scope reference is\n      published.\n    credentials_scope: per application, per environment\n    quote: >-\n      \"The type of access called 'OAuth 2.0 grant type' used for Equifax APIs is client\n      credentials - here the username and password are not required. Rather, you obtain\n      the Access Token by providing only the client_id, client_secret, and the scope.\"\nenvironments:\n  - name: Sandbox\n    base_url: https://api.sandbox.equifax.com\n    credentials: Sandbox Client ID/Secret, or an auto-generated Access Token on the app page\n    approval_required: false\n  - name: Test (UAT)\n    base_url: https://api.uat.equifax.com\n    credentials: Test Client ID/Secret, issued after \"Promote to Test\" approval (typically <48h)\n    approval_required: true\n  - name: Live (Production)\n    base_url:\
  \ https://api.equifax.com\n    credentials: Production Client ID/Secret, issued after a Go Live review\n    approval_required: true\n    additional_controls:\n      - IP allow-listing (IPv4 and IPv6, optional CIDR), configured per application\n      - Sectigo TLS certificates must be applied to production and lower environments\nadditional_credentials:\n  - name: Member number / subscriber ID + security code\n    applies_to: >-\n      Product-level credentials required by some Equifax products in addition to the OAuth\n      token (documented for Teletrack in the public quick-start guide).\n    source: https://assets.equifax.com/marketing/US/assets/developer-quick-start-guide.PDF\nfailure_modes:\n  - status: 401\n    meaning: Missing, invalid, or wrong-environment Access Token; request is not applied.\n  - status: 403\n    meaning: >-\n      Understood but permanently refused — insufficient rights to the resource, or the\n      calling gateway IP is not allow-listed for production.\ngaps:\n\
  \  - No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any\n    Equifax host (all 404 — see well-known/equifax-well-known.yml).\n  - No public scope reference; scope values require a portal sign-in.\n  - No published OpenAPI, so securitySchemes cannot be read from a contract.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equifax/refs/heads/main/authentication/equifax-authentication.yml
summary_line: 1 scheme
tags:
- Credit
- Credit History
- Credit Reporting
- Identity
- Fraud Detection
- Fortune 1000
---
