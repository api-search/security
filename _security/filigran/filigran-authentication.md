---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Filigran Authentication
name_suffix: Authentication
oauth_flows: []
overview: Filigran secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Filigran
provider_slug: filigran
scheme_count: 2
schemes:
- api: OpenCTI GraphQL API
  description: Each OpenCTI user has an API token (Profile > API access). Access rights are determined by the privileges of that user account. Content-Type application/json is required for GraphQL requests.
  format: 'Authorization: Bearer <API_TOKEN>'
  header: Authorization
  location: header
  name: OpenCTI bearer token
  scheme: bearer
  source: https://docs.opencti.io/latest/reference/api/
  type: http
- api: OpenAEV REST API
  description: OpenAEV (OpenBAS) REST API authenticates with a per-user bearer token, used by the official pyobas client.
  format: 'Authorization: Bearer <API_TOKEN>'
  header: Authorization
  location: header
  name: OpenAEV bearer token
  scheme: bearer
  source: https://docs.openaev.io/latest/
  type: http
slug: filigran-authentication
source_filename: filigran-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.opencti.io/latest/reference/api/ ; https://docs.openaev.io/latest/\ndocs: https://docs.opencti.io/latest/reference/api/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    API access to both OpenCTI and OpenAEV is via a per-user bearer API token\n    presented in the Authorization header. OAuth2 / OIDC / SAML are supported\n    for interactive user login (SSO) but the programmatic API uses static\n    bearer tokens, not OAuth scopes — so no scopes/ artifact is emitted.\nschemes:\n- name: OpenCTI bearer token\n  api: OpenCTI GraphQL API\n  type: http\n  scheme: bearer\n  location: header\n  header: Authorization\n  format: 'Authorization: Bearer <API_TOKEN>'\n  description: >-\n    Each OpenCTI user has an API token (Profile > API access). Access rights are\n    determined by the privileges of that user account. Content-Type\n    application/json is\
  \ required for GraphQL requests.\n  source: https://docs.opencti.io/latest/reference/api/\n- name: OpenAEV bearer token\n  api: OpenAEV REST API\n  type: http\n  scheme: bearer\n  location: header\n  header: Authorization\n  format: 'Authorization: Bearer <API_TOKEN>'\n  description: >-\n    OpenAEV (OpenBAS) REST API authenticates with a per-user bearer token, used\n    by the official pyobas client.\n  source: https://docs.openaev.io/latest/\nsso:\n  note: >-\n    Interactive platform login additionally supports OpenID Connect, SAML 2.0,\n    LDAP, and local authentication providers (user-login only, not API auth).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filigran/refs/heads/main/authentication/filigran-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Cybersecurity
- Threat Intelligence
- OpenCTI
- OpenAEV
- STIX
- GraphQL
- Breach and Attack Simulation
- Open Source
- Security
---
