---
api_key_in: []
api_specs:
- filename: zenlytic-embed-openapi.yml
  format: yaml
  label: Zenlytic Signed Embedding API
  slug: zenlytic-signed-embedding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenlytic/refs/heads/main/openapi/zenlytic-embed-openapi.yml
auth_types:
- http-basic
- sso-saml-oidc
- signed-jwt
description: ''
kind: authentication
layout: security
method: searched
name: Zenlytic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zenlytic secures its APIs with http-basic, sso-saml-oidc, and signed-jwt across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zenlytic
provider_slug: zenlytic
scheme_count: 4
schemes:
- detail: base64(client_id:client_secret) in the Authorization header; client_id/client_secret provisioned by a Zenlytic representative.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/zenlytic-embed-openapi.yml
  type: http
  used_by: Signed Embedding API (POST https://api.zenlytic.com/api/v1/embed/signed_url)
- detail: 'Workspace login via SSO. Documented providers: Microsoft Entra ID and Okta, with SSO-only enforcement, IP whitelisting, and custom JWT claim mapping. See docs authentication-and-security section.'
  docs: https://docs.zenlytic.com/authentication-and-security/sso-custom-claims-reference
  name: sso
  sources:
  - docs
  type: openIdConnect
- bearerFormat: JWT
  detail: Signed embed URLs carry a userJWT query parameter minted for the external_user_id; row/column access is scoped by user_attributes and role_name (embed | embed_with_sql | embedded_with_scheduling). Signed URLs expire (expires_in seconds).
  name: signedEmbedJwt
  scheme: bearer
  sources:
  - docs
  type: http
- detail: Warehouse connections support Google Workload Identity Federation (keyless BigQuery) and GitHub deploy keys for model repositories.
  docs: https://docs.zenlytic.com/authentication-and-security/google_workload_identity_federation
  name: warehouse-workload-identity
  sources:
  - docs
  type: mutualTLS
slug: zenlytic-authentication
source_filename: zenlytic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.zenlytic.com/embedding/signed_embedding\ndocs: https://docs.zenlytic.com/authentication-and-security/\nsummary:\n  types: [http-basic, sso-saml-oidc, signed-jwt]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Zenlytic has three distinct authentication surfaces: (1) the Signed\n    Embedding REST endpoint authenticates with HTTP Basic over client\n    credentials; (2) end users sign in to the app via SSO (Microsoft Entra,\n    Okta) or credentials; (3) embedded external users are carried by a signed\n    JWT minted by the signed-URL endpoint.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    used_by: Signed Embedding API (POST https://api.zenlytic.com/api/v1/embed/signed_url)\n    detail: base64(client_id:client_secret) in the Authorization header; client_id/client_secret provisioned by a Zenlytic representative.\n    sources: [openapi/zenlytic-embed-openapi.yml]\n  - name: sso\n  \
  \  type: openIdConnect\n    detail: >-\n      Workspace login via SSO. Documented providers: Microsoft Entra ID and\n      Okta, with SSO-only enforcement, IP whitelisting, and custom JWT claim\n      mapping. See docs authentication-and-security section.\n    docs: https://docs.zenlytic.com/authentication-and-security/sso-custom-claims-reference\n    sources: [docs]\n  - name: signedEmbedJwt\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    detail: >-\n      Signed embed URLs carry a userJWT query parameter minted for the\n      external_user_id; row/column access is scoped by user_attributes and\n      role_name (embed | embed_with_sql | embedded_with_scheduling). Signed\n      URLs expire (expires_in seconds).\n    sources: [docs]\n  - name: warehouse-workload-identity\n    type: mutualTLS\n    detail: >-\n      Warehouse connections support Google Workload Identity Federation\n      (keyless BigQuery) and GitHub deploy keys for model repositories.\n    docs: https://docs.zenlytic.com/authentication-and-security/google_workload_identity_federation\n\
  \    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenlytic/refs/heads/main/authentication/zenlytic-authentication.yml
summary_line: http-basic/sso-saml-oidc/signed-jwt · 4 schemes
tags:
- Company
- Commerce
- Business Intelligence
- Analytics
- Artificial Intelligence
- Data
- Embedded Analytics
- MCP
---
