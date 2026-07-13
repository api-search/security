---
api_key_in: []
api_specs:
- filename: Authentication_OpenAPI.json
  format: json
  label: Workday Authentication API
  slug: workday-authentication-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Authentication_OpenAPI.json
- filename: Identity_Management_OpenAPI.json
  format: json
  label: Workday Identity Management API
  slug: workday-identity-management-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Identity_Management_OpenAPI.json
- filename: Security_Groups_OpenAPI.json
  format: json
  label: Workday Security Groups API
  slug: workday-security-groups-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Security_Groups_OpenAPI.json
- filename: Audit_OpenAPI.json
  format: json
  label: Workday Audit and Compliance API
  slug: workday-audit-and-compliance-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Audit_OpenAPI.json
- filename: Privacy_OpenAPI.json
  format: json
  label: Workday Privacy API
  slug: workday-privacy-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Privacy_OpenAPI.json
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
