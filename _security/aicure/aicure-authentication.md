---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Aicure Authentication
name_suffix: Authentication
oauth_flows: []
overview: AiCure declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: AiCure
provider_slug: aicure
scheme_count: 3
schemes:
- api: OpenDBM REST API
  applied_to: Every operation on the main router carries dependencies=[Depends(get_current_active_user)]; only POST /odbm/v1/login is unauthenticated.
  evidence: https://github.com/AiCure/open_dbm/blob/master/rest_api/app/routers/router.py
  flow: password
  id: opendbm-oauth2-password
  scopes: []
  scopes_note: The token endpoint is FastAPI's OAuth2PasswordRequestForm. No scopes are declared or enforced anywhere in the published router or auth service, so there is no scope surface to catalog and scopes/ is deliberately absent.
  token_endpoint: POST /odbm/v1/login
  token_request_content_type: application/x-www-form-urlencoded
  token_request_fields:
  - grant_type=password
  - username
  - password
  token_response:
    access_token: JWT
    token_type: bearer
  type: oauth2
- algorithm: HS256
  api: OpenDBM REST API
  bearer_format: JWT
  evidence: https://github.com/AiCure/open_dbm/blob/master/rest_api/app/services/auth/auth.py
  header: 'Authorization: Bearer <token>'
  id: opendbm-bearer-jwt
  note: Tokens are signed and verified locally by the self-hosted instance. Because the deployment is the consumer's own, the signing secret, user store and token lifetime are all operator-owned; the shipped user store is a hard-coded dict (see sandbox/aicure-sandbox.yml).
  scheme: bearer
  type: http
- api: AiCure H.Code platform (not public)
  evidence_body: '{"message":"Missing Authentication Token"}'
  evidence_status: 403
  evidence_url: https://api.aicure.com/
  id: aicure-platform-gateway
  note: api.aicure.com resolves and is an AWS API Gateway, but every anonymous path returns 403 Missing Authentication Token, and AiCure publishes no developer documentation for it. The authentication model is not determinable from public material and has not been guessed here.
  status: gated
  type: unknown
slug: aicure-authentication
source_filename: aicure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://aicure.github.io/open_dbm/extras/odbm-rest-api\ndocs: https://aicure.github.io/open_dbm/extras/odbm-rest-api\nname: AiCure authentication profile\nsummary: >-\n  Two distinct authentication surfaces. The self-hosted OpenDBM REST API uses an OAuth2 password\n  grant that returns a JWT bearer token, applied to every operation except login. The commercial\n  AiCure platform (api.aicure.com) is closed: the AWS API Gateway rejects all anonymous traffic and\n  the customer sign-in flow at login.aicure.com is not documented publicly.\nschemes:\n- id: opendbm-oauth2-password\n  api: OpenDBM REST API\n  type: oauth2\n  flow: password\n  token_endpoint: POST /odbm/v1/login\n  token_request_content_type: application/x-www-form-urlencoded\n  token_request_fields:\n  - grant_type=password\n  - username\n  - password\n  token_response:\n    access_token: JWT\n    token_type: bearer\n  scopes: []\n  scopes_note: >-\n    The token\
  \ endpoint is FastAPI's OAuth2PasswordRequestForm. No scopes are declared or enforced\n    anywhere in the published router or auth service, so there is no scope surface to catalog and\n    scopes/ is deliberately absent.\n  applied_to: >-\n    Every operation on the main router carries dependencies=[Depends(get_current_active_user)];\n    only POST /odbm/v1/login is unauthenticated.\n  evidence: https://github.com/AiCure/open_dbm/blob/master/rest_api/app/routers/router.py\n- id: opendbm-bearer-jwt\n  api: OpenDBM REST API\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  header: 'Authorization: Bearer <token>'\n  algorithm: HS256\n  evidence: https://github.com/AiCure/open_dbm/blob/master/rest_api/app/services/auth/auth.py\n  note: >-\n    Tokens are signed and verified locally by the self-hosted instance. Because the deployment is\n    the consumer's own, the signing secret, user store and token lifetime are all operator-owned;\n    the shipped user store is a hard-coded dict\
  \ (see sandbox/aicure-sandbox.yml).\n- id: aicure-platform-gateway\n  api: AiCure H.Code platform (not public)\n  type: unknown\n  status: gated\n  evidence_url: https://api.aicure.com/\n  evidence_status: 403\n  evidence_body: '{\"message\":\"Missing Authentication Token\"}'\n  note: >-\n    api.aicure.com resolves and is an AWS API Gateway, but every anonymous path returns 403 Missing\n    Authentication Token, and AiCure publishes no developer documentation for it. The authentication\n    model is not determinable from public material and has not been guessed here.\nidentity_providers: []\nmtls: false\nopenid_connect: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aicure/refs/heads/main/authentication/aicure-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Healthcare
- Clinical Trials
- Medication Adherence
- Digital Biomarkers
- Digital Health
- Artificial Intelligence
- Computer-Vision
- Patient Engagement
- Life Sciences
- Open-Source
---
