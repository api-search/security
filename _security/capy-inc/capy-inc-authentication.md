---
api_key_in:
- body
api_specs:
- filename: capy-inc-captcha-openapi.yml
  format: yaml
  label: Lemin Captcha Verification API
  slug: lemin-captcha-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy-inc/refs/heads/main/openapi/capy-inc-captcha-openapi.yml
auth_types:
- apiKey
description: Lemin Captcha uses a two-key model. A public captcha_id (site key) identifies a configured captcha to the browser widget and is safe to expose client-side. A secret private_key authenticates the server-side verification call and must never be sent from the browser. The private_key is supplied in the JSON body of the verification request (not as an HTTP header), so it is not expressed as a standard OpenAPI securityScheme; the OpenAPI models it as a required request field. There is no OAuth surface.
kind: authentication
layout: security
method: searched
name: Capy Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capy Inc. secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Capy Inc.
provider_slug: capy-inc
scheme_count: 2
schemes:
- in: body
  name: private_key
  parameter: private_key
  role: server-side secret verification key (account key from the Lemin Dashboard)
  scope: server-to-server only
  sources:
  - https://help.leminnow.com/knowledge/verifying-a-lemin-captcha-answer
  type: apiKey
- in: client
  name: captcha_id
  parameter: captcha_id
  role: public site key identifying the captcha to the browser widget
  scope: client-side, non-secret
  sources:
  - https://help.leminnow.com/knowledge/displaying-lemin-captcha
  type: apiKey
slug: capy-inc-authentication
source_filename: capy-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://help.leminnow.com/knowledge/verifying-a-lemin-captcha-answer\ndocs: https://help.leminnow.com/knowledge/developers-guide\ndescription: >-\n  Lemin Captcha uses a two-key model. A public captcha_id (site key) identifies\n  a configured captcha to the browser widget and is safe to expose client-side.\n  A secret private_key authenticates the server-side verification call and must\n  never be sent from the browser. The private_key is supplied in the JSON body\n  of the verification request (not as an HTTP header), so it is not expressed as\n  a standard OpenAPI securityScheme; the OpenAPI models it as a required request\n  field. There is no OAuth surface.\nsummary:\n  types: [apiKey]\n  api_key_in: [body]\n  oauth2_flows: []\nschemes:\n- name: private_key\n  type: apiKey\n  in: body\n  parameter: private_key\n  role: server-side secret verification key (account key from the Lemin Dashboard)\n  scope: server-to-server\
  \ only\n  sources: [https://help.leminnow.com/knowledge/verifying-a-lemin-captcha-answer]\n- name: captcha_id\n  type: apiKey\n  in: client\n  parameter: captcha_id\n  role: public site key identifying the captcha to the browser widget\n  scope: client-side, non-secret\n  sources: [https://help.leminnow.com/knowledge/displaying-lemin-captcha]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capy-inc/refs/heads/main/authentication/capy-inc-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Security
- CAPTCHA
- Bot Detection
- Bot Prevention
- Fraud Prevention
- Account Takeover
- Authentication
- Web Security
- Developer Tools
---
