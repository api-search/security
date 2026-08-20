---
api_key_in:
- header
api_specs:
- filename: pendoio-account-api-openapi.yml
  format: yaml
  label: Pendo.io Account API
  slug: pendoio-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-account-api-openapi.yml
- filename: pendoio-admin-api-openapi.yml
  format: yaml
  label: Pendo.io Admin API
  slug: pendoio-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-admin-api-openapi.yml
- filename: pendoio-aggregation-api-openapi.yml
  format: yaml
  label: Pendo.io Aggregation API
  slug: pendoio-aggregation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-aggregation-api-openapi.yml
- filename: pendoio-bulk-deletion-gdpr-ccpa-api-openapi.yml
  format: yaml
  label: Pendo.io Bulk Deletion (GDPR/CCPA) API
  slug: pendoio-bulk-deletion-gdpr-ccpa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-bulk-deletion-gdpr-ccpa-api-openapi.yml
- filename: pendoio-conversations-api-openapi.yml
  format: yaml
  label: Pendo.io Conversations API
  slug: pendoio-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-conversations-api-openapi.yml
- filename: pendoio-data-sync-api-openapi.yml
  format: yaml
  label: Pendo.io Data Sync API
  slug: pendoio-data-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-data-sync-api-openapi.yml
- filename: pendoio-exclude-lists-servers-api-openapi.yml
  format: yaml
  label: Pendo.io Exclude Lists & Servers API
  slug: pendoio-exclude-lists-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-exclude-lists-servers-api-openapi.yml
- filename: pendoio-feature-api-openapi.yml
  format: yaml
  label: Pendo.io Feature API
  slug: pendoio-feature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-feature-api-openapi.yml
- filename: pendoio-guide-api-openapi.yml
  format: yaml
  label: Pendo.io Guide API
  slug: pendoio-guide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-guide-api-openapi.yml
- filename: pendoio-listen-api-openapi.yml
  format: yaml
  label: Pendo.io Listen API
  slug: pendoio-listen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-listen-api-openapi.yml
- filename: pendoio-metadata-api-openapi.yml
  format: yaml
  label: Pendo.io Metadata API
  slug: pendoio-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-metadata-api-openapi.yml
- filename: pendoio-page-api-openapi.yml
  format: yaml
  label: Pendo.io Page API
  slug: pendoio-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-page-api-openapi.yml
- filename: pendoio-report-api-openapi.yml
  format: yaml
  label: Pendo.io Report API
  slug: pendoio-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-report-api-openapi.yml
- filename: pendoio-segment-api-openapi.yml
  format: yaml
  label: Pendo.io Segment API
  slug: pendoio-segment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-segment-api-openapi.yml
- filename: pendoio-track-api-openapi.yml
  format: yaml
  label: Pendo.io Track API
  slug: pendoio-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-track-api-openapi.yml
- filename: pendoio-visitor-api-openapi.yml
  format: yaml
  label: Pendo.io Visitor API
  slug: pendoio-visitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-visitor-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pendoio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Pendo.io secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Pendo.io
provider_slug: pendoio
scheme_count: 2
schemes:
- description: Primary Engage API authentication. A per-subscription integration key created at https://app.pendo.io/admin/integrationkeys, sent in the x-pendo-integration-key request header. Verify a key with GET /api/v1/token/verify.
  in: header
  name: IntegrationKey
  parameter: x-pendo-integration-key
  sources:
  - openapi/pendoio-engage-openapi.yml
  type: apiKey
- code_challenge_methods_supported:
  - S256
  description: Pendo publishes RFC 8414 OAuth 2.0 Authorization Server metadata at https://app.pendo.io/.well-known/oauth-authorization-server. Supports the authorization_code (with PKCE S256), refresh_token, and client_credentials grants, plus RFC 7591 Dynamic Client Registration.
  flows:
  - authorizationUrl: https://app.pendo.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.pendo.io/oauth/v1/token
  - flow: clientCredentials
    tokenUrl: https://app.pendo.io/oauth/v1/token
  name: OAuth2
  registration_endpoint: https://app.pendo.io/oauth/v1/register
  sources:
  - well-known/pendoio-oauth-authorization-server.json
  type: oauth2
  userinfo_endpoint: https://app.pendo.io/oauth/v1/userinfo
slug: pendoio-authentication
source_filename: pendoio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/pendoio-engage-openapi.yml\ndocs: https://app.pendo.io/admin/integrationkeys\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: IntegrationKey\n  type: apiKey\n  in: header\n  parameter: x-pendo-integration-key\n  description: >-\n    Primary Engage API authentication. A per-subscription integration key created at\n    https://app.pendo.io/admin/integrationkeys, sent in the x-pendo-integration-key\n    request header. Verify a key with GET /api/v1/token/verify.\n  sources:\n  - openapi/pendoio-engage-openapi.yml\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Pendo publishes RFC 8414 OAuth 2.0 Authorization Server metadata at\n    https://app.pendo.io/.well-known/oauth-authorization-server. Supports the\n    authorization_code (with PKCE S256), refresh_token, and client_credentials\n    grants, plus RFC 7591\
  \ Dynamic Client Registration.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.pendo.io/oauth/authorize\n    tokenUrl: https://app.pendo.io/oauth/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://app.pendo.io/oauth/v1/token\n  registration_endpoint: https://app.pendo.io/oauth/v1/register\n  userinfo_endpoint: https://app.pendo.io/oauth/v1/userinfo\n  code_challenge_methods_supported:\n  - S256\n  sources:\n  - well-known/pendoio-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/authentication/pendoio-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Product Analytics
- Product Experience
- Digital Adoption
- User Analytics
- In-App Guidance
- Customer Feedback
- Software-as-a-Service
---
