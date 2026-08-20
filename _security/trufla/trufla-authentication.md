---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Trufla Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trufla declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Trufla
provider_slug: trufla
scheme_count: 0
schemes: []
slug: trufla-authentication
source_filename: trufla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://www.trufla.com/release-notes/truweb-release-notes-25-3-50\nnote: |\n  There is no public API and therefore no documented API authentication. This\n  artifact records what the provider's own public material reveals about the\n  platform's identity stack, so the absence is auditable rather than blank.\n  Deliberately NOT wired as a `type: Authentication` pointer in apis.yml — the\n  ergonomics check that pointer feeds asks whether API authentication is\n  documented for a consumer, and it is not.\napi_authentication:\n  documented: false\n  schemes: []\n  probes:\n  - {url: 'https://www.trufla.com/.well-known/openid-configuration', status: 404}\n  - {url: 'https://www.trufla.com/.well-known/oauth-authorization-server', status: 404}\n  - {url: 'https://www.trufla.com/.well-known/security.txt', status: 404}\n  note: No API key, bearer token, OAuth or mTLS documentation exists on any\n    resolving Trufla host.\nplatform_identity_stack:\n\
  \  observed: true\n  evidence:\n  - source: https://www.trufla.com/release-notes/truweb-release-notes-25-3-50\n    date: '2025-07-27'\n    detail: >-\n      truWeb 25.3.50 describes \"centralized authentication\", automated role\n      creation, enhanced permission enforcement, and \"improved alignment between\n      Keycloak and WordPress roles\" — Keycloak is the OIDC/OAuth 2.0 identity\n      provider behind the broker-facing products.\n  - source: https://www.trufla.com/release-notes/trumobile-11-0-update\n    detail: Clearer OTP security messaging and login report fixes — one-time\n      passcodes are part of the customer sign-in flow.\n  - source: https://www.trufla.com/release-notes/trumobile-9-0-update\n    detail: MFA reset fixes and jailbroken-iPhone detection in the truMobile\n      app.\n  - source: https://github.com/trufla-technology/AppAuth-Android\n    detail: The GitHub org forks openid/AppAuth-Android, the OAuth 2.0 / OpenID\n      Connect client SDK for Android — consistent\
  \ with an OIDC-backed mobile app.\n  - source: https://github.com/trufla-technology/jwt-auth\n    detail: The org also forks tymondesigns/jwt-auth, JWT authentication for\n      Laravel/Lumen — consistent with JWT-bearer service auth behind the\n      Laravel backend named in the truMobile release notes.\n  interpretation: >-\n    Keycloak-issued OIDC sessions for humans, JWT bearer tokens between Laravel\n    services, MFA/OTP on customer accounts. All of it is internal product\n    plumbing inferred from release notes and public forks — none of it is a\n    published, callable authentication contract, and no scope, token endpoint or\n    client-registration surface is exposed.\naccess_model:\n  self_serve: false\n  signup: https://www.trufla.com/request-a-demo/\n  gating: >-\n    Contract-gated. Access to truMarket/truMobile is sold to a brokerage; the\n    terms of service require the client to bring its own CSIO account and its\n    own insurer contracts and APIs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trufla/refs/heads/main/authentication/trufla-authentication.yml
summary_line: 0 schemes
tags:
- Insurance
- Canada
- Property and Casualty
- Insurtech
- Brokers
- Agency Management
- CSIO
- Policy Administration
- Quote Bind Issue
- Digital Distribution
---
