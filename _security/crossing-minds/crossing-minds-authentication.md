---
api_key_in: []
auth_types:
- http
description: The Crossing Minds B2B Recommendation API uses short-lived JWT bearer authentication (RFC 6750). Clients log in to obtain a JWT plus a refresh token scoped to a specific account and database, then present the JWT in the Authorization header. When the JWT expires, the refresh token is exchanged for a new JWT (and, when near expiry, a new refresh token) without re-submitting credentials.
kind: authentication
layout: security
method: searched
name: Crossing Minds Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crossing Minds secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crossing Minds
provider_slug: crossing-minds
scheme_count: 1
schemes:
- bearerFormat: JWT
  header: 'Authorization: Bearer <JWT_TOKEN>'
  name: bearerAuth
  scheme: bearer
  type: http
slug: crossing-minds-authentication
source_filename: crossing-minds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.api.crossingminds.com/authentication.html\ndocs: https://docs.api.crossingminds.com/authentication.html\nsummary:\n  types: [http]\n  http_scheme: bearer\n  bearer_format: JWT\n  standards: [RFC6750]\n  oauth2_flows: []\n  sso: [saml]\ndescription: >-\n  The Crossing Minds B2B Recommendation API uses short-lived JWT bearer\n  authentication (RFC 6750). Clients log in to obtain a JWT plus a refresh\n  token scoped to a specific account and database, then present the JWT in the\n  Authorization header. When the JWT expires, the refresh token is exchanged\n  for a new JWT (and, when near expiry, a new refresh token) without\n  re-submitting credentials.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    header: 'Authorization: Bearer <JWT_TOKEN>'\nlogin_flows:\n  - name: individual\n    endpoint: POST login/individual/\n    credentials: [email, password]\n    optional:\
  \ [db_id, db_name]\n  - name: service\n    endpoint: POST login/service/\n    credentials: [service_name, service_key]\n    optional: [db_id, db_name]\n    notes: Service accounts may hold multiple keys.\n  - name: sso-saml\n    endpoint: POST login/sso/saml/sp/\n    provider: OKTA\n    notes: SAML-based single sign-on.\n  - name: frontend-role\n    notes: >-\n      Login accepts frontend_user_id or frontend_session_id to restrict token\n      permissions to a specific end user or anonymous session.\nrefresh:\n  endpoint: POST login/refresh-token/\n  returns: A new short-lived JWT, and a new refresh token when the current one is near expiry.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossing-minds/refs/heads/main/authentication/crossing-minds-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai Ml
- Recommendations
- Personalization
- Machine Learning
- Recommender System
- Retrieval
- Ecommerce
---
