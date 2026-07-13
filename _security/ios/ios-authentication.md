---
api_key_in: []
api_specs:
- filename: app-store-connect-openapi.json
  format: json
  label: App Store Connect API
  slug: app-store-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ios/main/openapi/app-store-connect-openapi.json
- filename: app-store-server-notifications-asyncapi.yml
  format: yaml
  label: App Store Server Notifications
  slug: app-store-server-notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ios/main/asyncapi/app-store-server-notifications-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ios Authentication
name_suffix: Authentication
oauth_flows: []
overview: iOS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: iOS
provider_slug: ios
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: itc-bearer-token
  scheme: bearer
  sources:
  - openapi/app-store-connect-openapi.json
  type: http
slug: ios-authentication
source_filename: ios-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/app-store-connect-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: itc-bearer-token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/app-store-connect-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ios/refs/heads/main/authentication/ios-authentication.yml
summary_line: http · 1 scheme
tags:
- iOS
- Apple
- Mobile
- App Store
- Push Notifications
- In-App Purchases
- Subscriptions
- Authentication
- Wallet
- Developer Platform
---
