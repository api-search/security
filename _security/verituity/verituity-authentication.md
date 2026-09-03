---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Verituity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verituity declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Verituity
provider_slug: verituity
scheme_count: 2
schemes:
- credential_fields:
  - api_client_id
  - client_secret
  description: '"Creates an OAuth 2.0 machine-to-machine client scoped to the sandbox." Sandbox provisioning issues an api_client_id and a client_secret; the secret is shown once and, per the portal, "Verituity never retains it." The resulting access token is presented as `Authorization: Bearer <token>`.'
  flow: client_credentials
  id: oauth2_m2m
  scopes_note: The portal says the sandbox client is "scoped to the sandbox" but publishes no named scope list, so no scopes/ artifact is emitted rather than inventing one.
  scopes_published: false
  token_endpoint: null
  token_endpoint_note: NOT PUBLISHED. The portal names the grant but does not state a token URL, and neither host serves /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource (both 404). An integrator must obtain the token endpoint from Verituity directly.
  type: oauth2
- description: 'Certificate-bound access tokens per RFC 8705, presented as the production posture: "Switch to mTLS (RFC 8705, certificate-bound) before going live." The portal frames this as the control that satisfies strict federal identity assurance out of the box.'
  environment: production
  id: mtls
  standard: RFC 8705 (OAuth 2.0 Mutual-TLS Client Authentication and Certificate-Bound Access Tokens)
  type: mutualTLS
slug: verituity-authentication
source_filename: verituity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://verituity.com/developers\ndocs: https://verituity.com/developers\nnote: >-\n  DERIVED FROM DOCS, NOT FROM A SPEC. Verituity publishes no OpenAPI, so there are no\n  securitySchemes to read. Everything below is stated on Verituity's own developer portal, or was\n  observed on a live unauthenticated request to the published base URL.\nschemes:\n- id: oauth2_m2m\n  type: oauth2\n  flow: client_credentials\n  description: >-\n    \"Creates an OAuth 2.0 machine-to-machine client scoped to the sandbox.\" Sandbox provisioning\n    issues an api_client_id and a client_secret; the secret is shown once and, per the portal,\n    \"Verituity never retains it.\" The resulting access token is presented as\n    `Authorization: Bearer <token>`.\n  credential_fields:\n  - api_client_id\n  - client_secret\n  token_endpoint: null\n  token_endpoint_note: >-\n    NOT PUBLISHED. The portal names the grant but does not state a token URL,\
  \ and neither host\n    serves /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource\n    (both 404). An integrator must obtain the token endpoint from Verituity directly.\n  scopes_published: false\n  scopes_note: >-\n    The portal says the sandbox client is \"scoped to the sandbox\" but publishes no named scope\n    list, so no scopes/ artifact is emitted rather than inventing one.\n- id: mtls\n  type: mutualTLS\n  description: >-\n    Certificate-bound access tokens per RFC 8705, presented as the production posture:\n    \"Switch to mTLS (RFC 8705, certificate-bound) before going live.\" The portal frames this as\n    the control that satisfies strict federal identity assurance out of the box.\n  standard: RFC 8705 (OAuth 2.0 Mutual-TLS Client Authentication and Certificate-Bound Access Tokens)\n  environment: production\ntransport:\n  header: Authorization\n  format: Bearer <access_token>\n  observed_challenge: 'WWW-Authenticate: Bearer realm=\"verification-api-dev\"\
  '\nenvironments:\n- name: sandbox\n  base_url: https://platform.dev.verituityplatform.com/v1\n  auth: oauth2 client_credentials (bearer)\n  key_prefixes:\n    client_id: vc_sbx_\n    secret: sk_sbx_\n  note: >-\n    Prefixes are the documented FORMAT only; the portal states the keys its explorer generates are\n    examples that \"will not authenticate against the API.\"\n- name: production\n  base_url: null\n  auth: mTLS certificate-bound OAuth 2.0 (RFC 8705)\n  note: >-\n    No production base URL is published anywhere on verituity.com. Live access is arranged through\n    the demo/sales flow (\"Ask us about live sandbox access\").\nx-evidence:\n- url: https://verituity.com/developers\n  status: 200\n  note: developer portal; states OAuth 2.0 M2M, mTLS RFC 8705, one-time secret, per-client isolation\n- url: https://platform.dev.verituityplatform.com/v1/verifications\n  status: 401\n  note: >-\n    Live unauthenticated POST returned {\"error\":\"unauthorized\",\"status\":401} with\n  \
  \  WWW-Authenticate: Bearer realm=\"verification-api-dev\" (server: istio-envoy)\n- url: https://platform.dev.verituityplatform.com/.well-known/oauth-authorization-server\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verituity/refs/heads/main/authentication/verituity-authentication.yml
summary_line: 2 schemes
tags:
- Payments
- Payouts
- Disbursements
- Identity Verification
- Account Verification
- Fraud Prevention
- Payment Integrity
- Banking
- Financial Services
- Public Sector
- ISO 20022
- Compliance
- Company
---
