---
api_key_in: []
api_specs:
- filename: templafy-public-api-v3-openapi.json
  format: json
  label: Templafy Public API
  slug: templafy-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-public-api-v3-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Templafy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Templafy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Templafy
provider_slug: templafy
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/templafy-public-api-v3-openapi.json
  - openapi/templafy-public-api-v4-preview-openapi.json
  type: http
slug: templafy-authentication
source_filename: templafy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/templafy-public-api-v3-openapi.json + https://support.templafy.com/hc/en-us/articles/360008704477-Authentication-method\ndocs: https://support.templafy.com/hc/en-us/articles/4413600978577-API-Keys\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/templafy-public-api-v3-openapi.json\n  - openapi/templafy-public-api-v4-preview-openapi.json\ndetail: >-\n  The Templafy Public API authenticates with an API key sent as a bearer token\n  (`Authorization: Bearer <api-key>`). Keys are created, scoped, regenerated, and revoked in the\n  Templafy Admin Center under the Account > API Keys tab. Each key is issued with the specific\n  scopes / permissions it may use, and the same API Keys surface also issues tokens for SCIM 2.0\n  user and group provisioning. There is no OAuth 2.0 / OIDC authorization-code flow\
  \ — the key is a\n  static bearer credential managed per tenant.\nscopes_model: per-key scopes/permissions selected at key creation in the Admin Center\nscim: SCIM 2.0 provisioning tokens are issued from the same API Keys surface\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/authentication/templafy-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Document Generation
- Templates
- Content Management
- Digital Asset Management
- Document Automation
- Productivity
- Enterprise
- SaaS
---
