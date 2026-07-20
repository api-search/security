---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Edools Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edools secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Edools
provider_slug: edools
scheme_count: 1
schemes:
- description: API token credentials (token + secret combined) passed in the Authorization header using the Rails-style Token scheme.
  format: 'Authorization: Token token="CREDENTIALS"'
  header_name: Authorization
  in: header
  name: TokenAuth
  sources:
  - https://docs.edools.com/file.05_api.html
  type: apiKey
slug: edools-authentication
source_filename: edools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.edools.com/file.05_api.html\ndocs: https://docs.edools.com/file.05_api.html\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Token-based API key authentication. Each ApiKey has a token and a secret,\n    generated at creation; combined they form the \"credentials\". Credentials\n    are provisioned by Edools support on request. There is no OAuth surface.\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  header_name: Authorization\n  format: 'Authorization: Token token=\"CREDENTIALS\"'\n  description: >-\n    API token credentials (token + secret combined) passed in the Authorization\n    header using the Rails-style Token scheme.\n  sources: [https://docs.edools.com/file.05_api.html]\nversioning_header:\n  name: Accept\n  value: application/vnd.edools.core.v1+json\n  description: >-\n    API version is negotiated via a vendor Accept media type rather than a URL\n\
  \    path segment.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edools/refs/heads/main/authentication/edools-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Education
- E-Learning
- LMS
- Online Courses
- EdTech
- Content Management
- Digital Products
- Brazil
- REST
---
