---
api_key_in: []
api_specs:
- filename: canvas-lms-rest-api-openapi.yml
  format: yaml
  label: Canvas REST API
  slug: canvas-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-rest-api-openapi.yml
- filename: canvas-lms-live-events-asyncapi.yml
  format: yaml
  label: Canvas Live Events
  slug: canvas-live-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/openapi/canvas-lms-live-events-asyncapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Canvas Lms Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Canvas LMS secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Canvas LMS
provider_slug: canvas-lms
scheme_count: 2
schemes:
- description: Canvas OAuth2 (RFC 6749) authorization code grant. Register a Developer Key in the target Canvas account to obtain a client_id and client_secret.
  flows:
  - authorizationUrl: https://canvas.instructure.com/login/oauth2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://canvas.instructure.com/login/oauth2/token
  name: OAuth2
  sources:
  - openapi/canvas-lms-rest-api-openapi.yml
  type: oauth2
- description: A Canvas access token. For testing only — production apps MUST use the OAuth2 flow per the Canvas API Policy.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/canvas-lms-rest-api-openapi.yml
  type: http
slug: canvas-lms-authentication
source_filename: canvas-lms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/canvas-lms-rest-api-openapi.yml\ndocs:\n- https://developerdocs.instructure.com/services/canvas/oauth2/file.oauth.md\n- https://developerdocs.instructure.com/services/canvas/oauth2/file.oauth_endpoints.md\n- https://developerdocs.instructure.com/services/canvas/oauth2/file.developer_keys.md\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://canvas.instructure.com/login/oauth2/auth\n    tokenUrl: https://canvas.instructure.com/login/oauth2/token\n    scopes: 3\n  description: Canvas OAuth2 (RFC 6749) authorization code grant. Register a Developer Key in\n    the target Canvas account to obtain a client_id and client_secret.\n  sources:\n  - openapi/canvas-lms-rest-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: A Canvas access token. For testing\
  \ only — production apps MUST use the OAuth2\n    flow per the Canvas API Policy.\n  sources:\n  - openapi/canvas-lms-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canvas-lms/refs/heads/main/authentication/canvas-lms-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Learning Management
- Education
- EdTech
- LMS
- LTI
- Higher Education
- K-12
- Open Source
- AGPL
- Canvas
---
