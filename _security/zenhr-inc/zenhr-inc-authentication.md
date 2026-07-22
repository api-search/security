---
api_key_in: []
api_specs:
- filename: zenhr-inc-openapi.yml
  format: yaml
  label: ZenHR API
  slug: zenhr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenhr-inc/refs/heads/main/openapi/zenhr-inc-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zenhr Inc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ZenHR Inc secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ZenHR Inc
provider_slug: zenhr-inc
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.zenhr.com/en/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.zenhr.com/oauth/register
    scopes: 9
    tokenUrl: https://api.zenhr.com/en/oauth/token
  name: oauth2
  sources:
  - openapi/zenhr-inc-openapi.yml
  - https://api.zenhr.com/.well-known/oauth-authorization-server
  type: oauth2
slug: zenhr-inc-authentication
source_filename: zenhr-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# API Evangelist enrichment artifact\ngenerated: '2026-07-21'\nmethod: searched\nsource: openapi/zenhr-inc-openapi.yml\ndocs: https://api-docs.zenhr.com/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  token_placement: 'Authorization: Bearer'\n  pkce: S256\n  public_client: true\nnotes: 'OAuth 2.0 Authorization Code with PKCE (S256). Tokens presented as Authorization: Bearer. Integration apps are registered\n  by a Global Super Admin at /en/oauth/applications, granted per-scope authorities and a company data-access level. token_endpoint_auth_methods=none\n  (public client) per the published authorization-server metadata.'\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.zenhr.com/en/oauth/authorize\n    tokenUrl: https://api.zenhr.com/en/oauth/token\n    registrationUrl: https://api.zenhr.com/oauth/register\n    scopes: 9\n    pkce: S256\n  sources:\n  - openapi/zenhr-inc-openapi.yml\n\
  \  - https://api.zenhr.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenhr-inc/refs/heads/main/authentication/zenhr-inc-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Human Resources
- HR
- Payroll
- HRMS
- Employee Management
- MENA
- Attendance
- Time Off
- SaaS
---
