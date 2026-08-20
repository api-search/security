---
api_key_in:
- header
- query
api_specs:
- filename: salsify-digital-assets-api-openapi.yml
  format: yaml
  label: Salsify Digital Assets API
  slug: salsify-digital-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-digital-assets-api-openapi.yml
- filename: salsify-export-runs-api-openapi.yml
  format: yaml
  label: Salsify Export Runs API
  slug: salsify-export-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-export-runs-api-openapi.yml
- filename: salsify-imports-api-openapi.yml
  format: yaml
  label: Salsify Imports API
  slug: salsify-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-imports-api-openapi.yml
- filename: salsify-lists-api-openapi.yml
  format: yaml
  label: Salsify Lists API
  slug: salsify-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-lists-api-openapi.yml
- filename: salsify-org-id-api-openapi.yml
  format: yaml
  label: Salsify <org ID> API
  slug: salsify-org-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-org-id-api-openapi.yml
- filename: salsify-products-api-openapi.yml
  format: yaml
  label: Salsify Products API
  slug: salsify-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-products-api-openapi.yml
- filename: salsify-properties-api-openapi.yml
  format: yaml
  label: Salsify Properties API
  slug: salsify-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-properties-api-openapi.yml
- filename: salsify-record-types-api-openapi.yml
  format: yaml
  label: Salsify Record Types API
  slug: salsify-record-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-record-types-api-openapi.yml
- filename: salsify-records-api-openapi.yml
  format: yaml
  label: Salsify Records API
  slug: salsify-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/openapi/salsify-records-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Salsify Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Salsify secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Salsify
provider_slug: salsify
scheme_count: 2
schemes:
- in: header
  name: sec0
  parameter: Authorization
  sources:
  - openapi/salsify-api-settings-openapi.json
  - openapi/salsify-non-v1-endpoints-openapi.json
  - openapi/salsify-write-operations-openapi.json
  type: apiKey
- flows:
  - authorizationUrl: https://app.salsify.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://app.salsify.com/oauth/token
    tokenUrl: https://app.salsify.com/oauth/token
  name: OAuth2 (documented, not declared in OpenAPI)
  sources:
  - https://developers.salsify.com/docs/oauth2
  - well-known/salsify-oauth-authorization-server.json
  type: oauth2
slug: salsify-authentication
source_filename: salsify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/salsify-api-settings-openapi.json, openapi/salsify-non-v1-endpoints-openapi.json,\n  openapi/salsify-write-operations-openapi.json\ndocs: https://developers.salsify.com/docs/authentication-model\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\nmodels:\n- id: session\n  name: Session\n  applies_to: Interactive browser use only\n  description: >-\n    Username/password or SAML 2.0 SSO login stores a session cookie that expires after\n    one week, or after 24 hours of inactivity. Login is CAPTCHA-protected specifically\n    to prevent non-interactive session establishment.\n  rate_limit: 5,000 requests per hour, per user\n  docs: https://developers.salsify.com/docs/authentication-model\n- id: api-key\n  name: API Key\n  applies_to: Programmatic REST and GraphQL access\n  description: >-\n    Every Salsify user has an associated API key generated\
  \ on the My Profile page\n    (https://app.salsify.com/app/profile/edit/api). Sent as the Authorization request\n    header; also accepted as an access_token query parameter. The key inherits all of\n    that user's permissions and does not expire unless regenerated. Salsify recommends\n    a dedicated least-privilege integration user rather than a human account.\n  rate_limit: 10,000 requests per hour, per organization\n  docs: https://developers.salsify.com/reference/token-authentication-via-header-parameter\n- id: oauth2\n  name: OAuth 2.0\n  applies_to: Multi-tenant integrations acting on behalf of Salsify users\n  description: >-\n    Salsify is an OAuth 2.0 provider supporting only the Authorization Code grant.\n    OAuth applications are created by Salsify support (name + redirect URI) and are not\n    tied to a user or organization. Access tokens are Bearer tokens valid for 7200\n    seconds (2 hours); refresh tokens are single-use and are rotated on every refresh.\n  rate_limit:\
  \ 10,000 requests per hour, per organization\n  docs: https://developers.salsify.com/docs/oauth2\n- id: saml-sso\n  name: SAML 2.0 Single Sign-On\n  applies_to: Human login to the Salsify application\n  description: >-\n    SSO supported with AD FS 2.0, OneLogin, PingIdentity, Google Apps, Microsoft Entra ID,\n    Okta, and any other SAML 2.0 identity provider.\n  docs: https://developers.salsify.com/docs/sso-overview\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/salsify-api-settings-openapi.json\n  - openapi/salsify-non-v1-endpoints-openapi.json\n  - openapi/salsify-write-operations-openapi.json\n- name: OAuth2 (documented, not declared in OpenAPI)\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.salsify.com/oauth/authorize\n    tokenUrl: https://app.salsify.com/oauth/token\n    refreshUrl: https://app.salsify.com/oauth/token\n  sources:\n  - https://developers.salsify.com/docs/oauth2\n\
  \  - well-known/salsify-oauth-authorization-server.json\nauthorization_server_metadata:\n  file: well-known/salsify-oauth-authorization-server.json\n  spec: RFC 8414\n  issuer: https://app.salsify.com\n  code_challenge_methods_supported:\n  - S256\ngaps:\n- >-\n  The three published OpenAPI documents declare only the apiKey scheme (sec0). OAuth 2.0,\n  which the docs and the RFC 8414 metadata both confirm is live, is not modelled in any\n  securityScheme - so a spec-only reader under-reports Salsify's auth surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salsify/refs/heads/main/authentication/salsify-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Product Experience Management
- Product Information Management
- Digital Asset Management
- Commerce
- Retail
- Syndication
- Data Management
- Software-as-a-Service
---
