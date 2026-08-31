---
api_key_in: []
api_specs:
- filename: tarana-wireless-alerts-asyncapi.yml
  format: yaml
  label: Tarana Cloud Suite (TCS) Northbound API
  slug: tarana-cloud-suite-tcs-northbound-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tarana-wireless/refs/heads/main/asyncapi/tarana-wireless-alerts-asyncapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Tarana Wireless Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tarana Wireless declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Tarana Wireless
provider_slug: tarana-wireless
scheme_count: 4
schemes:
- authorization_server: https://idp.tcs.taranawireless.com
  discovery_document: false
  discovery_note: /.well-known/openid-configuration, /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource and /.well-known/jwks.json all return 404 on the IdP host. The authorization server publishes no discovery metadata, so an OAuth client cannot be configured without out-of-band instructions.
  evidence:
  - note: Named verbatim in the portal's env-config.js as the IdP response URL. The host answers unknown paths with {"error":"This URL doesn't exist on the authorization server."}, which confirms it is an OAuth 2.0 authorization server rather than a static host.
    status: 404
    url: https://idp.tcs.taranawireless.com/oauth2/idpresponse
  flow: authorization_code
  id: tcs-portal-session
  mfa: true
  mfa_evidence: The TCS event vocabulary defines an MFA_MANAGEMENT_OPERATIONS event type with three events, so multi-factor enrolment and management are first-class portal operations.
  surface: TCS operator portal (portal.tcs.taranawireless.com)
  type: oauth2
- evidence:
  - note: 'Body: "RBAC: access denied".'
    status: 403
    url: https://portal.tcs.taranawireless.com/northbound/swagger-ui.html
  - note: Public. Names security-service endpoints /api/tcs/v1/authorization and /api/tcs/v1/clients/key, and an apigw block whose apikey value is the literal placeholder SECRET_FROM_VAULT (no live secret is exposed).
    status: 200
    url: https://portal.tcs.taranawireless.com/operator-portal/env-config.js
  id: tcs-northbound-api-credential
  note: 'The credential type is NOT documented on any anonymously reachable Tarana surface and is deliberately not guessed here. Two pieces of real evidence bracket it: the portal''s own service map names a security-service exposing /api/tcs/v1/authorization and /api/tcs/v1/clients/key, which is the shape of a client-key issuance and authorization endpoint pair; and the TCS event vocabulary carries no separate API-token event type, which suggests keys are issued through the same operator/user management surface. Confirm against the TCS Administration Guide or the gated Swagger UI before integrating.'
  status: gated
  surface: TCS northbound REST API (portal.tcs.taranawireless.com/northbound)
  type: unknown
- evidence:
  - note: AWS API Gateway. Responds with x-amzn-errortype MissingAuthenticationTokenException and the body {"data":null,"error":{"code":403,"message":"The HTTP method or resources may not be supported.","status":"Unsupported API"}}. MissingAuthenticationTokenException is the standard AWS API Gateway response to an unsigned/unkeyed request. CORS access-control-allow-origin is pinned to https://portal.tcs.taranawireless.com, so this edge is provisioned for the first-party portal, not as a public developer API.
    status: 403
    url: https://api.tcs.taranawireless.com/
  id: tcs-api-gateway
  in: header
  status: gated
  surface: TCS API gateway (api.tcs.taranawireless.com)
  type: apiKey
- artifact: well-known/tarana-wireless-support-openid-configuration.json
  evidence:
  - note: 'Complete OpenID Provider Metadata: authorization, token, revocation, introspection, userinfo, registration and JWKS endpoints; RS256 id_token signing; DPoP signing algorithms advertised; client_secret_post / client_secret_basic / private_key_jwt token endpoint auth. Scopes are the Salesforce platform set, not Tarana product scopes.'
    status: 200
    url: https://support.taranawireless.com/.well-known/openid-configuration
  id: support-portal-oidc
  openIdConnectUrl: https://support.taranawireless.com/.well-known/openid-configuration
  scope: This governs sign-in to the customer support and knowledge portal only. It is NOT the authorization server for the TCS northbound API — that is idp.tcs.taranawireless.com.
  status: published
  surface: Salesforce Experience Cloud support portal (support.taranawireless.com)
  type: openIdConnect
slug: tarana-wireless-authentication
source_filename: tarana-wireless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: >-\n  Live anonymous probes of https://api.tcs.taranawireless.com/,\n  https://idp.tcs.taranawireless.com/, https://portal.tcs.taranawireless.com/northbound/,\n  https://support.taranawireless.com/.well-known/openid-configuration, plus the operator\n  portal's anonymous runtime configuration at\n  https://portal.tcs.taranawireless.com/operator-portal/env-config.js\nname: Tarana Wireless — authentication profile\nnote: >-\n  NO OpenAPI securitySchemes could be read: the TCS northbound OpenAPI sits behind the same\n  RBAC wall as the API itself, so derive-authentication.py had nothing to parse. Everything\n  below was established by probing the live edges and by reading the configuration Tarana\n  serves anonymously. Where a mechanism is implied but not stated by Tarana, it is marked\n  inferred and the evidence is named — nothing here is asserted from the shape of the URL\n  alone.\ngated: true\ngate: >-\n  The northbound API\
  \ reference (Swagger UI) and every Swagger/OpenAPI sibling path return\n  HTTP 403 with the plain-text body \"RBAC: access denied\" to anonymous callers. Credentials\n  are issued to an operator with a TCS tenant; there is no self-service developer signup.\nschemes:\n- id: tcs-portal-session\n  surface: TCS operator portal (portal.tcs.taranawireless.com)\n  type: oauth2\n  flow: authorization_code\n  authorization_server: https://idp.tcs.taranawireless.com\n  evidence:\n  - url: https://idp.tcs.taranawireless.com/oauth2/idpresponse\n    note: >-\n      Named verbatim in the portal's env-config.js as the IdP response URL. The host answers\n      unknown paths with {\"error\":\"This URL doesn't exist on the authorization server.\"},\n      which confirms it is an OAuth 2.0 authorization server rather than a static host.\n    status: 404\n  discovery_document: false\n  discovery_note: >-\n    /.well-known/openid-configuration, /.well-known/oauth-authorization-server,\n    /.well-known/oauth-protected-resource\
  \ and /.well-known/jwks.json all return 404 on the\n    IdP host. The authorization server publishes no discovery metadata, so an OAuth client\n    cannot be configured without out-of-band instructions.\n  mfa: true\n  mfa_evidence: >-\n    The TCS event vocabulary defines an MFA_MANAGEMENT_OPERATIONS event type with three\n    events, so multi-factor enrolment and management are first-class portal operations.\n- id: tcs-northbound-api-credential\n  surface: TCS northbound REST API (portal.tcs.taranawireless.com/northbound)\n  type: unknown\n  status: gated\n  note: >-\n    The credential type is NOT documented on any anonymously reachable Tarana surface and is\n    deliberately not guessed here. Two pieces of real evidence bracket it: the portal's own\n    service map names a security-service exposing /api/tcs/v1/authorization and\n    /api/tcs/v1/clients/key, which is the shape of a client-key issuance and authorization\n    endpoint pair; and the TCS event vocabulary carries no separate\
  \ API-token event type,\n    which suggests keys are issued through the same operator/user management surface. Confirm\n    against the TCS Administration Guide or the gated Swagger UI before integrating.\n  evidence:\n  - url: https://portal.tcs.taranawireless.com/northbound/swagger-ui.html\n    status: 403\n    note: 'Body: \"RBAC: access denied\".'\n  - url: https://portal.tcs.taranawireless.com/operator-portal/env-config.js\n    status: 200\n    note: >-\n      Public. Names security-service endpoints /api/tcs/v1/authorization and\n      /api/tcs/v1/clients/key, and an apigw block whose apikey value is the literal\n      placeholder SECRET_FROM_VAULT (no live secret is exposed).\n- id: tcs-api-gateway\n  surface: TCS API gateway (api.tcs.taranawireless.com)\n  type: apiKey\n  in: header\n  status: gated\n  evidence:\n  - url: https://api.tcs.taranawireless.com/\n    status: 403\n    note: >-\n      AWS API Gateway. Responds with x-amzn-errortype MissingAuthenticationTokenException\
  \ and\n      the body {\"data\":null,\"error\":{\"code\":403,\"message\":\"The HTTP method or resources may\n      not be supported.\",\"status\":\"Unsupported API\"}}. MissingAuthenticationTokenException is\n      the standard AWS API Gateway response to an unsigned/unkeyed request. CORS\n      access-control-allow-origin is pinned to https://portal.tcs.taranawireless.com, so this\n      edge is provisioned for the first-party portal, not as a public developer API.\n- id: support-portal-oidc\n  surface: Salesforce Experience Cloud support portal (support.taranawireless.com)\n  type: openIdConnect\n  openIdConnectUrl: https://support.taranawireless.com/.well-known/openid-configuration\n  artifact: well-known/tarana-wireless-support-openid-configuration.json\n  status: published\n  evidence:\n  - url: https://support.taranawireless.com/.well-known/openid-configuration\n    status: 200\n    note: >-\n      Complete OpenID Provider Metadata: authorization, token, revocation, introspection,\n\
  \      userinfo, registration and JWKS endpoints; RS256 id_token signing; DPoP signing\n      algorithms advertised; client_secret_post / client_secret_basic / private_key_jwt token\n      endpoint auth. Scopes are the Salesforce platform set, not Tarana product scopes.\n  scope: >-\n    This governs sign-in to the customer support and knowledge portal only. It is NOT the\n    authorization server for the TCS northbound API — that is idp.tcs.taranawireless.com.\noauth_scopes_published: false\noauth_scopes_note: >-\n  No Tarana-defined scope reference is reachable. The only scopes list found anywhere is the\n  Salesforce platform scope set in the support portal's OIDC metadata, which describes\n  Salesforce APIs and not Tarana's. scopes/ is deliberately not written rather than filled\n  with a foreign vocabulary.\nauthorization_model:\n  style: role-based access control (RBAC), enforced at the ingress\n  evidence: >-\n    Anonymous requests to gated paths are refused by the Istio ingress\
  \ with the literal\n    string \"RBAC: access denied\", and the portal env-config exposes an HBAC block with a\n    ROLES_WITH_GLOBAL_ACCESS list.\n  documented_roles:\n  - NOC Operator\n  - NOC L1 User\n  - OP Admin\n  roles_source: >-\n    Role names appear in Tarana's own operator-portal documentation surface; the machine\n    definition is not public.\n  hierarchy: >-\n    Access is additionally scoped by the network hierarchy the portal filters on — operator,\n    region, market, cell, site, sector, device — which is the same hierarchy carried on every\n    webhook payload.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tarana-wireless/refs/heads/main/authentication/tarana-wireless-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Networking
- Telecommunications
- Fixed Wireless Access
- Broadband
- Wireless
- Network Management
- Internet Service Providers
- CBRS
- Spectrum
- Telemetry
- Hardware
---
