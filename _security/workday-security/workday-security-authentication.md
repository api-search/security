---
api_key_in: []
api_specs:
- filename: workday-security-account-signons-api-openapi.yml
  format: yaml
  label: Workday Security Account Signons API
  slug: workday-security-account-signons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-account-signons-api-openapi.yml
- filename: workday-security-audit-logs-api-openapi.yml
  format: yaml
  label: Workday Security Audit Logs API
  slug: workday-security-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-audit-logs-api-openapi.yml
- filename: workday-security-authentication-configuration-api-openapi.yml
  format: yaml
  label: Workday Security Authentication Configuration API
  slug: workday-security-authentication-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-authentication-configuration-api-openapi.yml
- filename: workday-security-compliance-reports-api-openapi.yml
  format: yaml
  label: Workday Security Compliance Reports API
  slug: workday-security-compliance-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-compliance-reports-api-openapi.yml
- filename: workday-security-domain-security-policies-api-openapi.yml
  format: yaml
  label: Workday Security Domain Security Policies API
  slug: workday-security-domain-security-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-domain-security-policies-api-openapi.yml
- filename: workday-security-oauth-tokens-api-openapi.yml
  format: yaml
  label: Workday Security OAuth Tokens API
  slug: workday-security-oauth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-oauth-tokens-api-openapi.yml
- filename: workday-security-security-audit-api-openapi.yml
  format: yaml
  label: Workday Security Security Audit API
  slug: workday-security-security-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-security-audit-api-openapi.yml
- filename: workday-security-security-group-members-api-openapi.yml
  format: yaml
  label: Workday Security Security Group Members API
  slug: workday-security-security-group-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-security-group-members-api-openapi.yml
- filename: workday-security-security-groups-api-openapi.yml
  format: yaml
  label: Workday Security Security Groups API
  slug: workday-security-security-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-security-groups-api-openapi.yml
- filename: workday-security-sessions-api-openapi.yml
  format: yaml
  label: Workday Security Sessions API
  slug: workday-security-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-sessions-api-openapi.yml
- filename: workday-security-unidentified-signons-api-openapi.yml
  format: yaml
  label: Workday Security Unidentified Signons API
  slug: workday-security-unidentified-signons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-unidentified-signons-api-openapi.yml
- filename: workday-security-user-accounts-api-openapi.yml
  format: yaml
  label: Workday Security User Accounts API
  slug: workday-security-user-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-user-accounts-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workday Security Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Workday Security secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Workday Security
provider_slug: workday-security
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained from the Workday token endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/workday-security-audit-openapi.yml
  - openapi/workday-security-authentication-openapi.yml
  - openapi/workday-security-identity-management-openapi.yml
  - openapi/workday-security-security-groups-openapi.yml
  type: http
- description: OAuth 2.0 authorization code flow for obtaining access tokens to Workday REST APIs.
  flows:
  - authorizationUrl: https://{host}/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://{host}/ccx/oauth2/{tenant}/token
  name: oauth2
  sources:
  - openapi/workday-security-authentication-openapi.yml
  type: oauth2
slug: workday-security-authentication
source_filename: workday-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-security-audit-openapi.yml, openapi/workday-security-authentication-openapi.yml,\n  openapi/workday-security-identity-management-openapi.yml, openapi/workday-security-security-groups-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained from the Workday token endpoint.\n  sources:\n  - openapi/workday-security-audit-openapi.yml\n  - openapi/workday-security-authentication-openapi.yml\n  - openapi/workday-security-identity-management-openapi.yml\n  - openapi/workday-security-security-groups-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{host}/authorize\n    tokenUrl: https://{host}/ccx/oauth2/{tenant}/token\n    scopes: 3\n  description: OAuth 2.0 authorization code flow for\
  \ obtaining access tokens to Workday REST\n    APIs.\n  sources:\n  - openapi/workday-security-authentication-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/authentication/workday-security-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Access Control
- Audit
- Authentication
- Compliance
- Enterprise
- Identity Management
- Privacy
- SAML
- Security
- SSO
---
