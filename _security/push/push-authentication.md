---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Push Authentication
name_suffix: Authentication
oauth_flows: []
overview: Push declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Push
provider_slug: push
scheme_count: 1
schemes:
- description: 'Token-based authentication. The account secret (or master secret) is passed in the Authorization header after the literal string "Token token=". Example: `Authorization: Token token=dGVzdEBleGFtcGxlLmNvbTpsZXRtZWlu`.'
  format: Token token={{secret}}
  header_name: Authorization
  id: token
  in: header
  scheme: token
  type: http
  variants:
  - credential: account_secret / account_master_secret
    description: Account-level authentication for account-scoped resources.
    name: account
  - credential: app_secret
    description: App-level authentication for app-scoped resources.
    name: apps
slug: push-authentication
source_filename: push-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: http://developers.pushtech.com/api/authentication\napi: Cendyn CRM (PUSHTech) REST API\nbase_url: https://api.eu.cendyncrm.com\nschemes:\n- id: token\n  type: http\n  scheme: token\n  in: header\n  header_name: Authorization\n  format: 'Token token={{secret}}'\n  description: >-\n    Token-based authentication. The account secret (or master secret) is passed\n    in the Authorization header after the literal string \"Token token=\".\n    Example: `Authorization: Token token=dGVzdEBleGFtcGxlLmNvbTpsZXRtZWlu`.\n  variants:\n  - name: account\n    credential: account_secret / account_master_secret\n    description: Account-level authentication for account-scoped resources.\n  - name: apps\n    credential: app_secret\n    description: App-level authentication for app-scoped resources.\noauth2: false\nnotes: >-\n  No OAuth2 flow, token URL, or scopes are documented. Two authentication contexts\n  are supported (Account and Apps),\
  \ both using the same Authorization header shape.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/authentication/push-authentication.yml
summary_line: 1 scheme
tags:
- Company
- CRM
- Marketing Automation
- Hospitality
- Hotels
- Guest Experience
- Email
- SMS
- Push Notifications
- Webhooks
---
