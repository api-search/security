---
api_key_in:
- sdk-config
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Contextsdk Authentication
name_suffix: Authentication
oauth_flows: []
overview: ContextSDK secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ContextSDK
provider_slug: contextsdk
scheme_count: 1
schemes:
- description: Each app authenticates the ContextSDK integration with a license key created in the ContextSDK Dashboard. The key is passed to the SDK at initialization (for example ContextManager.applicationDidFinishLaunchingWithOptions(_:licenseKey:) on iOS, or ContextSDK.setup(context, licenseKey) on Android) and authorizes the ContextDecision and ContextPush products. Each environment / bundle ID or package name requires its own license key.
  in: sdk-config
  name: LicenseKey
  provisioning: https://dashboard.contextsdk.com/login
  sources:
  - https://docs.contextsdk.com/basics/getting-started
  type: apiKey
slug: contextsdk-authentication
source_filename: contextsdk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.contextsdk.com/basics/getting-started\ndocs: https://docs.contextsdk.com/basics/getting-started\nsummary:\n  types: [apiKey]\n  api_key_in: [sdk-config]\n  oauth2_flows: []\n  model: per-app license key\nschemes:\n- name: LicenseKey\n  type: apiKey\n  in: sdk-config\n  description: >-\n    Each app authenticates the ContextSDK integration with a license key created\n    in the ContextSDK Dashboard. The key is passed to the SDK at initialization\n    (for example ContextManager.applicationDidFinishLaunchingWithOptions(_:licenseKey:)\n    on iOS, or ContextSDK.setup(context, licenseKey) on Android) and authorizes\n    the ContextDecision and ContextPush products. Each environment / bundle ID or\n    package name requires its own license key.\n  provisioning: https://dashboard.contextsdk.com/login\n  sources: [https://docs.contextsdk.com/basics/getting-started]\nnotes: >-\n  ContextSDK has no public REST API and no\
  \ OpenAPI; there are no OAuth2 flows or\n  scopes. Authentication is a single per-app license key supplied to the client\n  SDK. On-device processing; data transmitted to ContextSDK servers is over\n  HTTPS/TLS 1.2+.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contextsdk/refs/heads/main/authentication/contextsdk-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Mobile
- SDK
- On-Device
- Context
- Machine Learning
- Push Notifications
- Privacy
- iOS
- Analytics
---
