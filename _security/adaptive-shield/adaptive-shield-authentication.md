---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Adaptive Shield Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adaptive Shield declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Adaptive Shield
provider_slug: adaptive-shield
scheme_count: 1
schemes:
- description: Per-user API key ("access token") generated from the dashboard user profile → API tab → Generate a new key. Every integrator that documents the connector asks only for the key and the regional domain, and none of them names the header, so the exact header name is not recorded here rather than guessed.
  evidence:
  - note: Key generation flow and the two regional domains.
    source: https://explained.tines.com/en/articles/8572857-adaptive-shield-authentication-guide
  - note: '"API Key" as the required credential; the key must have permission to log in to the API server and return data.'
    source: https://docs.axonius.com/docs/adaptive-shield
  - note: Regional base URLs and the v1 endpoint set the key is used against.
    source: https://docs.brinqa.com/docs/connectors/adaptive-shield/
  id: api_key
  in: header
  key_generation: Adaptive Shield dashboard → user profile → API tab → Generate a new key → name the key → Create.
  name: unknown
  scope_model: The key inherits the scope and permissions of the Adaptive Shield user account it was created under. No independent scopes or permission grants are published.
  type: apiKey
slug: adaptive-shield-authentication
source_filename: adaptive-shield-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nprovider: Adaptive Shield\nproviderId: adaptive-shield\nsource: >-\n  Tines, Torq, Brinqa and Axonius integration documentation for the Adaptive Shield API, plus live\n  probes of api.adaptive-shield.com. No first-party auth page survives: the Adaptive Shield help\n  centre is closed and developer.adaptive-shield.com no longer resolves.\ndocs: null\nsummary: >-\n  A single API-key scheme. The key is generated per user inside the Adaptive Shield dashboard and\n  inherits that user's scope and permissions — there is no separate service principal, no OAuth\n  authorization server, and no scope vocabulary.\nschemes:\n  - id: api_key\n    type: apiKey\n    in: header\n    name: unknown\n    description: >-\n      Per-user API key (\"access token\") generated from the dashboard user profile → API tab →\n      Generate a new key. Every integrator that documents the connector asks only for the key and\n      the regional domain, and none of\
  \ them names the header, so the exact header name is not\n      recorded here rather than guessed.\n    key_generation: >-\n      Adaptive Shield dashboard → user profile → API tab → Generate a new key → name the key → Create.\n    scope_model: >-\n      The key inherits the scope and permissions of the Adaptive Shield user account it was created\n      under. No independent scopes or permission grants are published.\n    evidence:\n      - source: https://explained.tines.com/en/articles/8572857-adaptive-shield-authentication-guide\n        note: Key generation flow and the two regional domains.\n      - source: https://docs.axonius.com/docs/adaptive-shield\n        note: >-\n          \"API Key\" as the required credential; the key must have permission to log in to the API\n          server and return data.\n      - source: https://docs.brinqa.com/docs/connectors/adaptive-shield/\n        note: Regional base URLs and the v1 endpoint set the key is used against.\noauth2: false\nopenid_connect:\
  \ false\nmutual_tls: false\nregions:\n  - region: US\n    base_url: https://api.adaptive-shield.com\n  - region: EU\n    base_url: https://eu.api.adaptive-shield.com\nlive_probe:\n  url: https://api.adaptive-shield.com/\n  status: 403\n  server: Adaptive\n  note: >-\n    Every unauthenticated path on both regional hosts returns an identical 134-byte 403 HTML body,\n    including the root. The host is up and enforcing auth; it does not emit a WWW-Authenticate\n    challenge, so no scheme can be confirmed from the wire.\nsso:\n  saml: true\n  provider_docs: https://learn.microsoft.com/en-us/entra/identity/saas-apps/adaptive-shield-tutorial\n  note: >-\n    SAML SSO for dashboard users (Microsoft Entra ID gallery application). This governs human login\n    to the console, not API authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-shield/refs/heads/main/authentication/adaptive-shield-authentication.yml
summary_line: 1 scheme
tags:
- SaaS Security
- SSPM
- Security Posture Management
- Cybersecurity
- Cloud Security
- Identity Management
- Compliance
---
