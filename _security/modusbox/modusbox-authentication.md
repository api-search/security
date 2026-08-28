---
api_key_in: []
api_specs:
- filename: modusbox-orca-contract-notice.yml
  format: yaml
  label: PortX ORCA (Open Reusable Core API)
  slug: portx-orca-open-reusable-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modusbox/refs/heads/main/openapi/modusbox-orca-contract-notice.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Modusbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: ModusBox declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ModusBox
provider_slug: modusbox
scheme_count: 2
schemes:
- bearer_format: JWT
  description: Bearer authentication using a signed JWT access token.
  header: Authorization
  id: jwt
  in: header
  primary: true
  scheme: bearer
  type: http
  value_prefix: 'Bearer '
- description: OpenID Connect authentication via the configured discovery endpoint.
  discovery_note: The discovery URL shipped in the published description is a localhost Keycloak realm placeholder, not a reachable issuer. This is consistent with ORCA being deployed as a per-institution connector where each deployment configures its own issuer, but it means the published contract does not name a real OIDC issuer an integrator could resolve.
  discovery_url_in_spec: http://localhost:8083/auth/realms/openbanking/.well-known/openid-configuration
  id: openIdConnect
  type: openIdConnect
slug: modusbox-authentication
source_filename: modusbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://orca-docs.portx.io/docs/getting-started/ (public Getting Started + Authentication\n  guide); security scheme names corroborated against the published ORCA OpenAPI description.\n\nsummary: >-\n  ORCA authenticates with a bearer JWT obtained through an OAuth 2.0 client_credentials\n  exchange. The published contract declares two alternative top-level security options —\n  an http/bearer JWT scheme and an openIdConnect scheme — so an institution may either\n  present a PortX-issued token or wire the connector to its own OIDC issuer. Credentials\n  are not self-service: PortX documents that a Client ID, Client Secret and API Key are\n  obtained by contacting a PortX representative.\n\ncredential_acquisition:\n  self_service: false\n  signup_url: https://portx.io/contact\n  process: >-\n    \"Contact your PortX representative to obtain: Client ID, Client Secret, API Key\"\n    (Getting Started). There is no developer\
  \ signup, no free tier and no key-issuance\n    console. Production use additionally requires a separately executed commercial\n    agreement with PortX per the ORCA licence.\n  credentials_issued:\n  - Client ID\n  - Client Secret\n  - API Key\n\nschemes:\n- id: jwt\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  header: Authorization\n  value_prefix: 'Bearer '\n  description: Bearer authentication using a signed JWT access token.\n  primary: true\n- id: openIdConnect\n  type: openIdConnect\n  description: OpenID Connect authentication via the configured discovery endpoint.\n  discovery_url_in_spec: http://localhost:8083/auth/realms/openbanking/.well-known/openid-configuration\n  discovery_note: >-\n    The discovery URL shipped in the published description is a localhost Keycloak realm\n    placeholder, not a reachable issuer. This is consistent with ORCA being deployed as a\n    per-institution connector where each deployment configures its own issuer, but it\n\
  \    means the published contract does not name a real OIDC issuer an integrator could\n    resolve.\n\ntoken_flow:\n  protocol: OAuth 2.0\n  grant_type: client_credentials\n  token_endpoint_documented: https://auth.portx.io/oauth/token\n  token_endpoint_resolves: false\n  token_endpoint_note: >-\n    auth.portx.io does not resolve in DNS (NXDOMAIN, probed 2026-08-26). As with\n    api.portx.io, the documented host appears illustrative; a real deployment issues\n    tokens from the issuer configured for that institution's connector.\n  request_content_type: application/json\n  request_fields:\n  - client_id\n  - client_secret\n  - grant_type\n  response: 'bearer access token presented as `Authorization: Bearer <token>`'\n\nscopes:\n  published: false\n  note: >-\n    No OAuth scopes are declared. Both security schemes are applied with empty scope\n    arrays and no scope reference page exists in the documentation, so no scopes/\n    artifact is written — there is no scope surface to record.\n\
  \nrequest_context_headers:\n  note: >-\n    Beyond authentication, ORCA carries deployment context in headers rather than in the\n    token, which an integrator must supply per call.\n  headers:\n  - name: servicerId\n    required: false\n    purpose: Account servicer identification (the bank).\n  - name: servicerBranchId\n    required: false\n    purpose: Account servicer identification at branch or centre level.\n\ntransport_security:\n  tls_required: true\n  mtls: >-\n    Not declared in the ORCA contract. PortX does ship automated mTLS management for\n    Integration Manager hosted APIs (announced on the PortX blog), which is a platform\n    capability rather than an ORCA contract requirement.\n\ngaps:\n- No self-service credential issuance; every integrator needs a sales conversation.\n- The documented token host and API host do not resolve.\n- The OIDC discovery URL in the published contract is a localhost placeholder.\n- No scopes, so authorisation granularity is not expressible\
  \ in the contract.\n- No documented token lifetime, refresh behaviour or rotation guidance.\n\nx-evidence:\n- url: https://orca-docs.portx.io/docs/getting-started/\n  status: 200\n- url: https://auth.portx.io/oauth/token\n  status: 0\n  note: DNS resolution failed (NXDOMAIN)\n- url: https://portx.io/contact\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modusbox/refs/heads/main/authentication/modusbox-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Banking
- Core Banking
- Credit Unions
- Financial Services
- Integration
- iPaaS
- Payments
- ISO 20022
- Open Banking
- Data
---
