---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Mirus Authentication
name_suffix: Authentication
oauth_flows: []
overview: MiRus declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MiRus
provider_slug: mirus
scheme_count: 1
schemes:
- bearer_format: JWT
  documented_by_provider: false
  evidence: 'The public app bundle contains `API_URL:"https://rpm.mirusmed.com"`, an axios `baseURL="https://rpm.mirusmed.com"`, `Authorization`/`Bearer` header construction and two `cognito` references. Every /api/* route answers `401` with `WWW-Authenticate: Bearer`.'
  id: bearer_jwt
  identity_provider: AWS Cognito
  scheme: bearer
  type: http
slug: mirus-authentication
source_filename: mirus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: derived\nsource: >-\n  https://rpm.mirusmed.com/js/app.d85d3fa1.js (the provider's own public, unauthenticated\n  JavaScript bundle) plus anonymous HTTP probes of https://rpm.mirusmed.com/api/*\nnote: >-\n  MiRus publishes NO authentication documentation, no developer portal and no OpenAPI. This\n  profile is derived from the provider's public application bundle and from the challenge the\n  API itself returns to anonymous callers. Because nothing here is documented BY MiRus, no\n  `type: Authentication` pointer is wired into apis.yml — the artifact records what was\n  observed, it does not credit MiRus with publishing an auth reference.\napi: GALILEO RPM / \"Mirus Analytics\" application backend (not a published developer API)\nbase: https://rpm.mirusmed.com\nschemes:\n- id: bearer_jwt\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  identity_provider: AWS Cognito\n  evidence: >-\n    The public app bundle contains `API_URL:\"https://rpm.mirusmed.com\"\
  `, an axios\n    `baseURL=\"https://rpm.mirusmed.com\"`, `Authorization`/`Bearer` header construction and two\n    `cognito` references. Every /api/* route answers `401` with `WWW-Authenticate: Bearer`.\n  documented_by_provider: false\nprobes:\n- url: https://rpm.mirusmed.com/api/org\n  status: 401\n  www_authenticate: Bearer\n- url: https://rpm.mirusmed.com/api/org/clinician\n  status: 401\n  www_authenticate: Bearer\n- url: https://rpm.mirusmed.com/api/org/report\n  status: 401\n  www_authenticate: Bearer\n- url: https://rpm.mirusmed.com/api/org/emrpush\n  status: 401\n  www_authenticate: Bearer\n- url: https://rpm.mirusmed.com/api/org/insurance\n  status: 401\n  www_authenticate: Bearer\n- url: https://rpm.mirusmed.com/api/org/compliance\n  status: 401\n  www_authenticate: Bearer\n- url: https://rpm.mirusmed.com/api/admin/device\n  status: 401\n  www_authenticate: Bearer\n- url: https://rpm.mirusmed.com/api/v1/fhir\n  status: 401\n  www_authenticate: Bearer\n- url: https://rpm.mirusmed.com/api/v1/fhir/metadata\n\
  \  status: 401\n  www_authenticate: Bearer\n- url: https://rpm.mirusmed.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://rpm.mirusmed.com/.well-known/openid-configuration\n  status: 404\n- url: https://rpm.mirusmed.com/.well-known/smart-configuration\n  status: 404\nscopes:\n  documented: false\n  note: >-\n    No OAuth scope reference is published and no authorization-server metadata is served, so\n    scopes/ is deliberately not written rather than filled with a guess.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirus/refs/heads/main/authentication/mirus-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Medical Devices
- Healthcare
- Life Sciences
- Spine
- Orthopaedics
- Structural Heart
- Remote Patient Monitoring
- Medical Implants
- Surgical Planning
---
