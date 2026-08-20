---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Centaur Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Centaur Labs declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Centaur Labs
provider_slug: centaur-labs
scheme_count: 2
schemes:
- description: Your Centaur API key, sent on every request.
  id: APIKeyHeader
  in: header
  name: X-API-KEY
  type: apiKey
- description: Bearer token obtained from the authentication endpoint (POST /auth/public/v1/login) by supplying the API Key and API Password. Tokens can be verified (POST /auth/public/v1/testToken), rotated (POST /auth/public/v1/refreshToken) and revoked (POST /auth/public/v1/logout).
  id: BearerToken
  scheme: bearer
  type: http
slug: centaur-labs-authentication
source_filename: centaur-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.centaurlabs.com/reference/security + OpenAPI securitySchemes embedded in docs.centaurlabs.com/reference/*\napi: Centaur Public API\ndocs: https://docs.centaurlabs.com/reference/security\nserver: https://api.centaurlabs.com\nsummary: >-\n  The Centaur public API authenticates with an API Key sent in the X-API-KEY\n  header. Session-based endpoints additionally issue a short-lived bearer token\n  obtained by exchanging the API Key and API Password at the login endpoint.\n  Credentials (one API Key + one API Password per account) are generated in the\n  Centaur Portal under Organization Settings > API Integration.\nschemes:\n- id: APIKeyHeader\n  type: apiKey\n  in: header\n  name: X-API-KEY\n  description: Your Centaur API key, sent on every request.\n- id: BearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token obtained from the authentication endpoint\n    (POST /auth/public/v1/login) by\
  \ supplying the API Key and API Password.\n    Tokens can be verified (POST /auth/public/v1/testToken), rotated\n    (POST /auth/public/v1/refreshToken) and revoked (POST /auth/public/v1/logout).\ncredentials:\n- name: API Key\n  provisioning: Portal > Organization Settings > API Integration > Generate API Key\n  note: Displayed once; store securely.\n- name: API Password\n  provisioning: Portal > Organization Settings > API Integration > Generate New Password\n  note: One password per account; regenerating invalidates the previous one.\noauth2: false\nopenidconnect: false\nmutualtls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centaur-labs/refs/heads/main/authentication/centaur-labs-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Data Annotation
- Data Labeling
- Machine-Learning
- Healthcare
- Medical Imaging
- Training Data
---
