---
api_key_in: []
auth_types:
- http
description: The Sydecar API authenticates every request with a Bearer token supplied on the HTTP Authorization header. Tokens are issued as API keys tied to a single API user account (one account may hold more than one key). Sydecar provisions production API tokens on sign-up and issues separate sandbox/staging tokens on request, so credentials are scoped per environment. Captured from the public Sydecar API "Overview and Guide" documentation.
kind: authentication
layout: security
method: searched
name: Sydecar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sydecar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sydecar
provider_slug: sydecar
scheme_count: 1
schemes:
- description: All API calls authenticate via a Bearer token on the Authorization header. Each API key is associated with a single API user account, though one API user account can control more than one API key.
  format: 'Authorization: Bearer <api_key>'
  header: Authorization
  location: header
  name: bearerAuth
  scheme: bearer
  source: https://api-docs.sydecar.io/docs/resources/guide/
  type: http
slug: sydecar-authentication
source_filename: sydecar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api-docs.sydecar.io/docs/resources/guide/\nsummary:\n  types:\n  - http\ndescription: >-\n  The Sydecar API authenticates every request with a Bearer token supplied on\n  the HTTP Authorization header. Tokens are issued as API keys tied to a single\n  API user account (one account may hold more than one key). Sydecar provisions\n  production API tokens on sign-up and issues separate sandbox/staging tokens on\n  request, so credentials are scoped per environment. Captured from the public\n  Sydecar API \"Overview and Guide\" documentation.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  location: header\n  header: Authorization\n  format: 'Authorization: Bearer <api_key>'\n  description: >-\n    All API calls authenticate via a Bearer token on the Authorization header.\n    Each API key is associated with a single API user account, though one API\n    user account can control more than one API key.\n\
  \  source: https://api-docs.sydecar.io/docs/resources/guide/\nenvironments:\n- name: production\n  notes: >-\n    A single production environment per account, tied to ledger and fund\n    management activities on behalf of your SPVs. Production API tokens are\n    provided when you sign up for the service.\n- name: staging\n  notes: >-\n    As many staging (development) environments as required. Each staging\n    environment has a single API user, with one or more API keys. Sandbox tokens\n    are provided on request for testing.\ndocs:\n- https://api-docs.sydecar.io/docs/resources/guide/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sydecar/refs/heads/main/authentication/sydecar-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Financial Services
- Fintech
- Venture Capital
- SPV
- Investment
- Compliance
- API
---
