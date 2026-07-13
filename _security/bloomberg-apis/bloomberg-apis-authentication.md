---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bloomberg Apis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bloomberg APIs secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bloomberg APIs
provider_slug: bloomberg-apis
scheme_count: 3
schemes:
- description: 'Desktop API authorization is handled by the local Bloomberg Professional

    terminal. Applications open a session against `localhost:8194` and the

    terminal context is the authorization. No token is presented over the wire.'
  in: header
  name: desktopAPI
  parameter: X-BLPAPI-Session
  sources:
  - openapi/bloomberg-blpapi-openapi.yml
  type: apiKey
- description: 'Server API authorization is by ASID and registered IP address.

    The application''s IP must be entitled in the Bloomberg Anywhere

    permissioning system; an `AuthorizationRequest` with `ipAddress`

    validates the user''s identity at that location.'
  in: header
  name: serverAPI
  parameter: X-BLPAPI-ASID
  sources:
  - openapi/bloomberg-blpapi-openapi.yml
  type: apiKey
- bearerFormat: BLPAPI-Token
  description: 'B-PIPE applications acquire a token via the

    `AuthorizationTokenRequest` operation, then submit the token in an

    `AuthorizationRequest` to obtain an Identity object. The Identity

    object is then attached to subsequent service requests.'
  name: bpipeToken
  scheme: bearer
  sources:
  - openapi/bloomberg-blpapi-openapi.yml
  type: http
slug: bloomberg-apis-authentication
source_filename: bloomberg-apis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bloomberg-blpapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: desktopAPI\n  type: apiKey\n  in: header\n  parameter: X-BLPAPI-Session\n  description: |-\n    Desktop API authorization is handled by the local Bloomberg Professional\n    terminal. Applications open a session against `localhost:8194` and the\n    terminal context is the authorization. No token is presented over the wire.\n  sources:\n  - openapi/bloomberg-blpapi-openapi.yml\n- name: serverAPI\n  type: apiKey\n  in: header\n  parameter: X-BLPAPI-ASID\n  description: |-\n    Server API authorization is by ASID and registered IP address.\n    The application's IP must be entitled in the Bloomberg Anywhere\n    permissioning system; an `AuthorizationRequest` with `ipAddress`\n    validates the user's identity at that location.\n  sources:\n  - openapi/bloomberg-blpapi-openapi.yml\n- name: bpipeToken\n \
  \ type: http\n  scheme: bearer\n  bearerFormat: BLPAPI-Token\n  description: |-\n    B-PIPE applications acquire a token via the\n    `AuthorizationTokenRequest` operation, then submit the token in an\n    `AuthorizationRequest` to obtain an Identity object. The Identity\n    object is then attached to subsequent service requests.\n  sources:\n  - openapi/bloomberg-blpapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/authentication/bloomberg-apis-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Analytics
- Financial Data
- Market Data
- News
- Terminal
---
