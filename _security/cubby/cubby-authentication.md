---
api_key_in: []
auth_types: []
description: Cubby runs two distinct authentication models on one host. The Operator and Storefront APIs use a long-lived, out-of-band-issued API key presented as an HTTP bearer token, scoped to an Organization and further constrained by one of eight named key roles plus a separate PII entitlement. The MCP server on the same host uses OAuth 2.1 with PKCE and dynamic client registration. There is no self-service credential issuance for the REST surface — keys are obtained by emailing support.
kind: authentication
layout: security
method: searched
name: Cubby Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cubby declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cubby
provider_slug: cubby
scheme_count: 2
schemes:
- applies_to:
  - Cubby Operator API
  - Cubby Storefront API
  contact: support@cubbystorage.com
  expiry: not documented
  format: Bearer <api-key>
  header: Authorization
  id: operator_api_key
  in: header
  issuance: Out of band. "In order to obtain an API key, please contact support@cubbystorage.com." API access additionally requires an executed Order under the Cubby API Terms of Service, so the credential is commercially gated, not self-service.
  note: The storefront web components take the same key as a `data-api-key` attribute on a <script> tag, which places a Storefront-role key in client-side HTML by design. That makes the role separation load-bearing rather than advisory — see roles below.
  rotation: not documented
  scheme: bearer
  scoping: Credentials attach conceptually to the Organization and carry access to all resources (managers, facilities, customers, leases) visible to that Organization.
  self_service: false
  type: http
- applies_to:
  - Cubby MCP Server
  authorization_endpoint: https://api.cubbystorage.com/oauth/authorize
  discovery:
  - path: /.well-known/oauth-authorization-server
    spec: RFC 8414
    status: 200
  - path: /.well-known/oauth-protected-resource
    spec: RFC 9728
    status: 200
  dynamic_client_registration: true
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  id: mcp_oauth
  issuer: https://api.cubbystorage.com
  method: probed
  pkce:
    required_methods:
    - S256
  registration_endpoint: https://api.cubbystorage.com/connect/register
  scopes:
  - mcp
  token_endpoint: https://api.cubbystorage.com/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: cubby-authentication
source_filename: cubby-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://cubbystorage.github.io/docs/api/#authentication\ndocs: https://cubbystorage.github.io/docs/api/#authentication\ndescription: >-\n  Cubby runs two distinct authentication models on one host. The Operator and Storefront\n  APIs use a long-lived, out-of-band-issued API key presented as an HTTP bearer token,\n  scoped to an Organization and further constrained by one of eight named key roles plus\n  a separate PII entitlement. The MCP server on the same host uses OAuth 2.1 with PKCE and\n  dynamic client registration. There is no self-service credential issuance for the REST\n  surface — keys are obtained by emailing support.\nschemes:\n- id: operator_api_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <api-key>'\n  applies_to:\n  - Cubby Operator API\n  - Cubby Storefront API\n  issuance: >-\n    Out of band. \"In order to obtain an API key, please contact support@cubbystorage.com.\"\
  \n    API access additionally requires an executed Order under the Cubby API Terms of Service,\n    so the credential is commercially gated, not self-service.\n  contact: support@cubbystorage.com\n  rotation: not documented\n  expiry: not documented\n  self_service: false\n  scoping: >-\n    Credentials attach conceptually to the Organization and carry access to all resources\n    (managers, facilities, customers, leases) visible to that Organization.\n  note: >-\n    The storefront web components take the same key as a `data-api-key` attribute on a\n    <script> tag, which places a Storefront-role key in client-side HTML by design. That\n    makes the role separation load-bearing rather than advisory — see roles below.\n- id: mcp_oauth\n  type: oauth2\n  flow: authorizationCode\n  applies_to:\n  - Cubby MCP Server\n  authorization_endpoint: https://api.cubbystorage.com/oauth/authorize\n  token_endpoint: https://api.cubbystorage.com/oauth/token\n  registration_endpoint: https://api.cubbystorage.com/connect/register\n\
  \  issuer: https://api.cubbystorage.com\n  grant_types:\n  - authorization_code\n  - refresh_token\n  pkce:\n    required_methods:\n    - S256\n  token_endpoint_auth_methods:\n  - none\n  dynamic_client_registration: true\n  scopes:\n  - mcp\n  discovery:\n  - path: /.well-known/oauth-authorization-server\n    spec: RFC 8414\n    status: 200\n  - path: /.well-known/oauth-protected-resource\n    spec: RFC 9728\n    status: 200\n  method: probed\nroles:\n  model: named key roles, one per issued API key\n  description: >-\n    \"API keys are issued with a specific role that determines which endpoints and operations\n    are accessible.\" The roles reference table in the docs enumerates the endpoints reachable\n    under each role.\n  values:\n  - name: Manager\n    summary: >-\n      Most comprehensive. Read and write across leases, customers, leads, payments, units,\n      coverage, auctions, notes, tasks, pricing groups and reports; read access to access\n      codes, discounts, facilities,\
  \ facility groups, ledgers, organizations and payment methods.\n  - name: Search\n  - name: Storefront\n  - name: Report\n  - name: Coverages\n  - name: Access Codes\n  - name: Communication\n  - name: Locks\npii_entitlement:\n  documented: true\n  behaviour: >-\n    PII access is a separate entitlement on the key, not a role. \"If your API key does not\n    have access to PII, all PII fields will be skipped in API responses.\" Fields are silently\n    omitted rather than masked or rejected, so a client must not treat a missing field as a\n    missing value.\n  fields:\n  - customer names\n  - customer addresses\n  - customer phone numbers\n  - customer email addresses\n  - customer date of birth\n  - customer ID numbers\n  - alternative contact names\n  - alternative contact phone numbers\n  - alternative contact email addresses\n  - vehicle license numbers\n  - vehicle states\ngaps:\n- No documented key rotation, expiry or revocation procedure for the Operator API key.\n- No self-service\
  \ credential issuance; every key requires a support email and a signed Order.\n- No OAuth or OIDC on the REST surface — OAuth exists only for the MCP server.\n- No mTLS, no request signing, no IP allowlisting documented.\nx-evidence:\n  fetched: '2026-08-11'\n  url: https://cubbystorage.github.io/docs/api/\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubby/refs/heads/main/authentication/cubby-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Self Storage
- Property Management
- Facility Management
- Real Estate
- Payments
- SaaS
- Artificial Intelligence
- Revenue Management
- E-Commerce
---
