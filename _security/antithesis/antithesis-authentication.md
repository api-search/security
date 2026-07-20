---
api_key_in: []
auth_types:
- http
- openIdConnect
description: 'Antithesis isolates each customer into a tenant with its own cloud instance. Four actions require authorization: pushing images to the Antithesis registry, kicking off tests, viewing reports, and multiverse debugging. Automated actions (image push, launching tests via the webhook/REST API) use long-lived machine credentials; interactive actions (viewing reports, multiverse debugging) use SSO. There is no OpenAPI to derive from; this profile is captured from the docs.'
kind: authentication
layout: security
method: searched
name: Antithesis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Antithesis secures its APIs with http and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Antithesis
provider_slug: antithesis
scheme_count: 4
schemes:
- description: Machine credentials (a webhook `user` and `password`) generated per tenant and sent securely at signup. Used by CI to launch tests via the webhook / REST API. Long-lived; rotatable by Antithesis on compromise. Should not be used in manual/interactive processes.
  name: webhookBasicAuth
  scheme: basic
  source: https://antithesis.com/docs/configuration/auth/
  type: http
  used_for:
  - launch tests
  - push images
- description: Container image registry credentials (JSON key file) for pushing images to the tenant's Antithesis image registry.
  in: file
  name: registryCredentials
  parameter_name: $TENANT_NAME.key.json
  source: https://antithesis.com/docs/configuration/auth/
  type: apiKey
- description: 'Login with GitHub for user access to reports and multiverse debugging. Authorization criteria: organization membership, team membership, public repo collaborators, or verified email domain.'
  name: ssoGitHub
  scheme: github-sso
  source: https://antithesis.com/docs/configuration/auth/
  type: openIdConnect
  used_for:
  - view reports
  - multiverse debugging
- description: Login with any OIDC-compliant Identity Provider (Okta, Microsoft Entra, Google Identity). Customer supplies client ID/secret and issuer URL / .well-known endpoint; Antithesis supplies the redirect URL.
  name: ssoOIDC
  openIdConnectUrl: https://{tenant}.antithesis.com/oidc/callback
  source: https://antithesis.com/docs/configuration/auth/
  type: openIdConnect
  used_for:
  - view reports
  - multiverse debugging
slug: antithesis-authentication
source_filename: antithesis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://antithesis.com/docs/configuration/auth/\ndocs: https://antithesis.com/docs/configuration/auth/\ndescription: >-\n  Antithesis isolates each customer into a tenant with its own cloud instance.\n  Four actions require authorization: pushing images to the Antithesis registry,\n  kicking off tests, viewing reports, and multiverse debugging. Automated actions\n  (image push, launching tests via the webhook/REST API) use long-lived machine\n  credentials; interactive actions (viewing reports, multiverse debugging) use\n  SSO. There is no OpenAPI to derive from; this profile is captured from the docs.\nsummary:\n  types: [http, openIdConnect]\n  http_schemes: [basic]\n  sso: [github, oidc]\nschemes:\n  - name: webhookBasicAuth\n    type: http\n    scheme: basic\n    description: >-\n      Machine credentials (a webhook `user` and `password`) generated per tenant\n      and sent securely at signup. Used by CI to launch tests\
  \ via the webhook /\n      REST API. Long-lived; rotatable by Antithesis on compromise. Should not be\n      used in manual/interactive processes.\n    used_for: [launch tests, push images]\n    source: https://antithesis.com/docs/configuration/auth/\n  - name: registryCredentials\n    type: apiKey\n    in: file\n    parameter_name: $TENANT_NAME.key.json\n    description: >-\n      Container image registry credentials (JSON key file) for pushing images to\n      the tenant's Antithesis image registry.\n    source: https://antithesis.com/docs/configuration/auth/\n  - name: ssoGitHub\n    type: openIdConnect\n    scheme: github-sso\n    description: >-\n      Login with GitHub for user access to reports and multiverse debugging.\n      Authorization criteria: organization membership, team membership, public\n      repo collaborators, or verified email domain.\n    used_for: [view reports, multiverse debugging]\n    source: https://antithesis.com/docs/configuration/auth/\n  - name: ssoOIDC\n\
  \    type: openIdConnect\n    openIdConnectUrl: https://{tenant}.antithesis.com/oidc/callback\n    description: >-\n      Login with any OIDC-compliant Identity Provider (Okta, Microsoft Entra,\n      Google Identity). Customer supplies client ID/secret and issuer URL /\n      .well-known endpoint; Antithesis supplies the redirect URL.\n    used_for: [view reports, multiverse debugging]\n    source: https://antithesis.com/docs/configuration/auth/\nnotes: >-\n  Reports are served only via unguessable signed URLs; SSO can additionally gate\n  report access. Multiverse debugging requires SSO. Support / credential requests:\n  support@antithesis.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antithesis/refs/heads/main/authentication/antithesis-authentication.yml
summary_line: http/openIdConnect · 4 schemes
tags:
- Company
- Developer Tools
- Testing
- Software Testing
- Deterministic Simulation
- Fuzzing
- Reliability
- Distributed Systems
- SDK
---
