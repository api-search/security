---
api_key_in: []
api_specs:
- filename: aps-sdk-openapi
  format: yaml
  label: Autodesk Fusion API
  slug: autodesk-fusion-api
  spec_type: OpenAPI
  url: https://github.com/autodesk-platform-services/aps-sdk-openapi
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Autodesk Fusion Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
overview: Autodesk Fusion secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and implicit flow(s).
provider_name: Autodesk Fusion
provider_slug: autodesk-fusion
scheme_count: 4
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
  name: 2-legged
  sources:
  - openapi/accountadmin.yaml
  - openapi/authentication.yaml
  - openapi/datamanagement.yaml
  - openapi/issues.yaml
  - openapi/modelderivative.yaml
  - openapi/oss.yaml
  - openapi/secureserviceaccount.yaml
  - openapi/webhooks.yaml
  type: oauth2
- flows:
  - flow: implicit
    scopes: 0
  name: 3-legged-implicit
  sources:
  - openapi/accountadmin.yaml
  - openapi/issues.yaml
  type: oauth2
- flows:
  - flow: authorizationCode
    scopes: 0
  name: 3-legged
  sources:
  - openapi/accountadmin.yaml
  - openapi/authentication.yaml
  - openapi/datamanagement.yaml
  - openapi/issues.yaml
  - openapi/modelderivative.yaml
  - openapi/oss.yaml
  - openapi/webhooks.yaml
  type: oauth2
- description: Basic Authorization by providing client id and client secret.
  name: client-credentials
  scheme: basic
  sources:
  - openapi/authentication.yaml
  - openapi/secureserviceaccount.yaml
  type: http
slug: autodesk-fusion-authentication
source_filename: autodesk-fusion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/accountadmin.yaml, openapi/authentication.yaml, openapi/datamanagement.yaml,\n  openapi/issues.yaml, openapi/modelderivative.yaml, openapi/oss.yaml, openapi/secureserviceaccount.yaml,\n  openapi/webhooks.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\nschemes:\n- name: 2-legged\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    scopes: 0\n  sources:\n  - openapi/accountadmin.yaml\n  - openapi/authentication.yaml\n  - openapi/datamanagement.yaml\n  - openapi/issues.yaml\n  - openapi/modelderivative.yaml\n  - openapi/oss.yaml\n  - openapi/secureserviceaccount.yaml\n  - openapi/webhooks.yaml\n- name: 3-legged-implicit\n  type: oauth2\n  flows:\n  - flow: implicit\n    scopes: 0\n  sources:\n  - openapi/accountadmin.yaml\n  - openapi/issues.yaml\n- name: 3-legged\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    scopes: 0\n  sources:\n\
  \  - openapi/accountadmin.yaml\n  - openapi/authentication.yaml\n  - openapi/datamanagement.yaml\n  - openapi/issues.yaml\n  - openapi/modelderivative.yaml\n  - openapi/oss.yaml\n  - openapi/webhooks.yaml\n- name: client-credentials\n  type: http\n  scheme: basic\n  description: Basic Authorization by providing client id and client secret.\n  sources:\n  - openapi/authentication.yaml\n  - openapi/secureserviceaccount.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk-fusion/refs/heads/main/authentication/autodesk-fusion-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- CAD
- CAM
- CAE
- Manufacturing
- Design Automation
- GraphQL
- REST
- Autodesk Platform Services
---
