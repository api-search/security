---
api_key_in:
- sdk-key
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Reforge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reforge secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Reforge
provider_slug: reforge
scheme_count: 2
schemes:
- description: 'Server-side SDK key with full access to the environment''s configuration and flag data. Passed to the SDK at init (Reforge.init(sdk_key: "<SDK-KEY>")) or via the REFORGE_BACKEND_SDK_KEY environment variable.'
  env: REFORGE_BACKEND_SDK_KEY
  in: sdk-key
  legacy_env: PREFAB_API_KEY
  name: BackendSdkKey
  sources:
  - https://docs.reforge.com/docs/tutorials/get-started
  type: apiKey
- description: Client/mobile SDK key restricted to single-user flag evaluation; hides raw flag rules and configuration data so it is safe to ship in browser/mobile clients.
  in: sdk-key
  name: FrontendSdkKey
  sources:
  - https://docs.reforge.com/docs/tutorials/get-started
  type: apiKey
slug: reforge-authentication
source_filename: reforge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.reforge.com/docs/tutorials/get-started\ndocs: https://docs.reforge.com/docs/tutorials/get-started\nsummary:\n  types: [apiKey]\n  api_key_in: [sdk-key]\n  oauth2_flows: []\n  note: >-\n    Reforge is SDK-key authenticated; there is no OAuth authorization surface, so\n    no scopes/ artifact applies.\nschemes:\n- name: BackendSdkKey\n  type: apiKey\n  in: sdk-key\n  env: REFORGE_BACKEND_SDK_KEY\n  legacy_env: PREFAB_API_KEY\n  description: >-\n    Server-side SDK key with full access to the environment's configuration and\n    flag data. Passed to the SDK at init (Reforge.init(sdk_key: \"<SDK-KEY>\")) or\n    via the REFORGE_BACKEND_SDK_KEY environment variable.\n  sources: [https://docs.reforge.com/docs/tutorials/get-started]\n- name: FrontendSdkKey\n  type: apiKey\n  in: sdk-key\n  description: >-\n    Client/mobile SDK key restricted to single-user flag evaluation; hides raw\n    flag rules and configuration\
  \ data so it is safe to ship in browser/mobile\n    clients.\n  sources: [https://docs.reforge.com/docs/tutorials/get-started]\nkey_management:\n  displayed_once: true\n  storage: secure hash only\n  rotation: generate an additional key, then retire the old one\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reforge/refs/heads/main/authentication/reforge-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Feature Flags
- Feature Management
- Dynamic Configuration
- Live Config
- Experimentation
- Developer Tools
- SDK
- Observability
---
