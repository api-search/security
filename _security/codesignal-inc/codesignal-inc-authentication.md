---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Codesignal Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodeSignal, Inc. secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CodeSignal, Inc.
provider_slug: codesignal-inc
scheme_count: 1
schemes:
- description: CodeSignal GraphQL and Webhook APIs authenticate with a static API key sent as an HTTP Authorization header formatted "Bearer [example key]". API keys are provisioned per-company; existing customers request keys via support@codesignal.com. Per-key permissions gate operations (insufficient scope yields an Access Denied error).
  format: Bearer [example key]
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - https://developer.codesignal.com/graphql
  type: http
slug: codesignal-inc-authentication
source_filename: codesignal-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.codesignal.com/graphql\ndocs: https://developer.codesignal.com/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    CodeSignal GraphQL and Webhook APIs authenticate with a static API key sent\n    as an HTTP Authorization header formatted \"Bearer [example key]\". API keys\n    are provisioned per-company; existing customers request keys via\n    support@codesignal.com. Per-key permissions gate operations (insufficient\n    scope yields an Access Denied error).\n  header: Authorization\n  format: Bearer [example key]\n  sources: [https://developer.codesignal.com/graphql]\nnotes: >-\n  No OpenAPI is published (the primary surface is GraphQL at\n  https://app.codesignal.com/graphql). Webhook deliveries are separately\n  verified with an X-CodeSignal-Signature HMAC-SHA256 header over\
  \ the endpoint\n  URL + event type + timestamp using a per-endpoint secret.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codesignal-inc/refs/heads/main/authentication/codesignal-inc-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Business Applications
- Technical Assessment
- Developer Hiring
- Skills Assessment
- Technical Interviews
- GraphQL
- Webhooks
- Talent
---
