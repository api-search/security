---
api_key_in: []
auth_types: []
description: 'Authentication profile for the Wolf staffing-platform API, derived from the published developer documentation. Wolf is multi-tenant: every request must carry a tenant key plus one of two credentials — a platform API key (acting on behalf of the staffing company / tenant) or a user authentication token (acting on behalf of a job seeker or client). No OAuth 2.0 / OpenID Connect authorization server is documented.'
kind: authentication
layout: security
method: searched
name: Wolf Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wolf declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Wolf
provider_slug: wolf
scheme_count: 2
schemes:
- description: Platform API key identifying the staffing company (tenant). Used when acting on behalf of the tenant (e.g. reading tenant configuration, updating client profiles, pushing unique-coordinate updates). Documented as always safe to include to avoid access-denied responses. Treated like a password; rotating it causes significant downtime.
  id: platform_api_key
  in: header
  name: Authentication
  scope: tenant
  type: apiKey
- description: Per-user authentication_token returned by POST /sign_in. Required for actions taken on behalf of a user (job seeker or client) — viewing jobs, applying, check-in / check-out, availability, chat. User type must be 'freelancer' to access jobs.
  id: user_auth_token
  in: header
  issued_by:
    method: POST
    operation: sign_in
    returns: user.authentication_token
    url: https://api.wolf.xyz/api/v1/sign_in
  name: Authentication
  scope: user
  type: apiKey
slug: wolf-authentication
source_filename: wolf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.fromwolf.com/glossary/core-attributes-of-all-api\ndocs: https://docs.fromwolf.com/user-api/authentication-api\ndescription: >-\n  Authentication profile for the Wolf staffing-platform API, derived from the\n  published developer documentation. Wolf is multi-tenant: every request must\n  carry a tenant key plus one of two credentials — a platform API key (acting on\n  behalf of the staffing company / tenant) or a user authentication token\n  (acting on behalf of a job seeker or client). No OAuth 2.0 / OpenID Connect\n  authorization server is documented.\nbase_url: https://api.wolf.xyz/api/v1/\nmulti_tenant: true\ntenant_key:\n  required: true\n  description: >-\n    Tenant (staffing company) identifier, supplied on every call. Most tenant\n    keys end in '_db' (e.g. 'brandname_db'). Obtained from the tenant / account\n    manager; cannot be self-issued.\n  location: request body / query parameter\n  parameter:\
  \ tenant\nschemes:\n- id: platform_api_key\n  type: apiKey\n  in: header\n  name: Authentication\n  scope: tenant\n  description: >-\n    Platform API key identifying the staffing company (tenant). Used when acting\n    on behalf of the tenant (e.g. reading tenant configuration, updating client\n    profiles, pushing unique-coordinate updates). Documented as always safe to\n    include to avoid access-denied responses. Treated like a password; rotating\n    it causes significant downtime.\n- id: user_auth_token\n  type: apiKey\n  in: header\n  name: Authentication\n  scope: user\n  description: >-\n    Per-user authentication_token returned by POST /sign_in. Required for actions\n    taken on behalf of a user (job seeker or client) — viewing jobs, applying,\n    check-in / check-out, availability, chat. User type must be 'freelancer' to\n    access jobs.\n  issued_by:\n    operation: sign_in\n    method: POST\n    url: https://api.wolf.xyz/api/v1/sign_in\n    returns: user.authentication_token\n\
  oauth2: false\nopenid_connect: false\nmutual_tls: false\nnotes:\n- Keys are issued out-of-band by the tenant / account manager; there is no\n  self-service key portal documented.\n- One-time-password (OTP) is supported as an optional sign-in factor\n  (request_one_time_password + one_time_password field on sign_in).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wolf/refs/heads/main/authentication/wolf-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Staffing
- Gig Economy
- Workforce Management
- Jobs
- Scheduling
- On-Demand Staffing
- Chat
---
