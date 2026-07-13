---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Autodesk Bim360 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
overview: Autodesk BIM 360 secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and implicit flow(s).
provider_name: Autodesk BIM 360
provider_slug: autodesk-bim360
scheme_count: 3
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
  name: 2-legged
  sources:
  - openapi/autodesk-bim360-account-admin-openapi.yml
  - openapi/autodesk-bim360-issues-openapi.yml
  type: oauth2
- flows:
  - flow: implicit
    scopes: 0
  name: 3-legged-implicit
  sources:
  - openapi/autodesk-bim360-account-admin-openapi.yml
  - openapi/autodesk-bim360-issues-openapi.yml
  type: oauth2
- flows:
  - flow: authorizationCode
    scopes: 0
  name: 3-legged
  sources:
  - openapi/autodesk-bim360-account-admin-openapi.yml
  - openapi/autodesk-bim360-issues-openapi.yml
  type: oauth2
slug: autodesk-bim360-authentication
source_filename: autodesk-bim360-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/autodesk-bim360-account-admin-openapi.yml, openapi/autodesk-bim360-issues-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\nschemes:\n- name: 2-legged\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    scopes: 0\n  sources:\n  - openapi/autodesk-bim360-account-admin-openapi.yml\n  - openapi/autodesk-bim360-issues-openapi.yml\n- name: 3-legged-implicit\n  type: oauth2\n  flows:\n  - flow: implicit\n    scopes: 0\n  sources:\n  - openapi/autodesk-bim360-account-admin-openapi.yml\n  - openapi/autodesk-bim360-issues-openapi.yml\n- name: 3-legged\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    scopes: 0\n  sources:\n  - openapi/autodesk-bim360-account-admin-openapi.yml\n  - openapi/autodesk-bim360-issues-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk-bim360/refs/heads/main/authentication/autodesk-bim360-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- Construction
- Project Management
- BIM
- Document Management
- Field Management
- Issues Tracking
- Cost Management
- Model Coordination
- RFIs
- Checklists
---
