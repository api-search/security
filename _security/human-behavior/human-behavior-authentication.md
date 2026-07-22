---
api_key_in:
- client-sdk-init
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Human Behavior Authentication
name_suffix: Authentication
oauth_flows: []
overview: Human Behavior secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Human Behavior
provider_slug: human-behavior
scheme_count: 1
schemes:
- description: Project API key provided to HumanBehaviorTracker.init(). Configurable options include ingestionUrl, redactionStrategy, and redactFields.
  in: sdk-init
  name: projectApiKey
  parameter: apiKey
  sources:
  - https://docs.humanbehavior.co/docs/sdk
  type: apiKey
slug: human-behavior-authentication
source_filename: human-behavior-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.humanbehavior.co/docs/sdk\ndocs: https://docs.humanbehavior.co/docs/sdk\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - client-sdk-init\n  oauth2_flows: []\n  notes: >-\n    Human Behavior authenticates via a project API key passed to the JavaScript\n    SDK at initialization: HumanBehaviorTracker.init('YOUR_API_KEY', options?).\n    The key identifies the project whose sessions and events are ingested. No\n    public REST API, OAuth flow, or documented server-side securityScheme was\n    found; auth is scoped to the client-side ingestion SDK.\nschemes:\n- name: projectApiKey\n  type: apiKey\n  in: sdk-init\n  parameter: apiKey\n  description: >-\n    Project API key provided to HumanBehaviorTracker.init(). Configurable\n    options include ingestionUrl, redactionStrategy, and redactFields.\n  sources:\n  - https://docs.humanbehavior.co/docs/sdk\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/human-behavior/refs/heads/main/authentication/human-behavior-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Analytics
- Product Analytics
- Session Replay
- Artificial Intelligence
- Developer Tools
- SDK
---
