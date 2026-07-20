---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bitfount Authentication
name_suffix: Authentication
oauth_flows:
- interactive-login
overview: Bitfount secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the interactive-login flow(s).
provider_name: Bitfount
provider_slug: bitfount
scheme_count: 2
schemes:
- description: Default mechanism. Running a pod or SDK session opens a browser-based login against the Bitfount Hub access manager (am.hub.bitfount.com); the user authenticates and the SDK caches the resulting access token for subsequent API calls to hub.bitfount.com.
  name: InteractiveLogin
  sources:
  - https://docs.bitfount.com/guides/SDK/for-data-custodians/setting-up/authentication-authorisation-options
  type: oauth2
- description: Non-interactive alternative for unattended pods. Each pod can be assigned a key pair (accessKeyID + accessKey) created in the Bitfount Hub under My Pods > API Keys. The pod authenticates on initialisation using these values, avoiding the interactive web login.
  fields:
  - accessKeyID
  - accessKey
  managed_at: https://hub.bitfount.com/
  name: PodApiKeys
  sources:
  - https://docs.bitfount.com/guides/SDK/for-data-custodians/setting-up/authentication-authorisation-options
  type: apiKey
slug: bitfount-authentication
source_filename: bitfount-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.bitfount.com/guides/SDK/for-data-custodians/setting-up/authentication-authorisation-options\ndocs: https://docs.bitfount.com/guides/SDK/for-data-custodians/setting-up/authentication-authorisation-options\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [interactive-login]\n  identity_host: am.hub.bitfount.com\nschemes:\n- name: InteractiveLogin\n  type: oauth2\n  description: >-\n    Default mechanism. Running a pod or SDK session opens a browser-based login\n    against the Bitfount Hub access manager (am.hub.bitfount.com); the user\n    authenticates and the SDK caches the resulting access token for subsequent\n    API calls to hub.bitfount.com.\n  sources: [https://docs.bitfount.com/guides/SDK/for-data-custodians/setting-up/authentication-authorisation-options]\n- name: PodApiKeys\n  type: apiKey\n  description: >-\n    Non-interactive alternative for unattended pods. Each pod can\
  \ be assigned a\n    key pair (accessKeyID + accessKey) created in the Bitfount Hub under\n    My Pods > API Keys. The pod authenticates on initialisation using these\n    values, avoiding the interactive web login.\n  fields: [accessKeyID, accessKey]\n  managed_at: https://hub.bitfount.com/\n  sources: [https://docs.bitfount.com/guides/SDK/for-data-custodians/setting-up/authentication-authorisation-options]\nnotes: >-\n  Bitfount publishes no public OpenAPI spec; the SDK wraps a private REST API on\n  hub.bitfount.com. This profile is captured from the documentation, not derived\n  from a machine-readable security scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitfount/refs/heads/main/authentication/bitfount-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Federated Learning
- Machine Learning
- Data Science
- Privacy
- Artificial Intelligence
- Healthcare
- Python SDK
- Data Collaboration
---
