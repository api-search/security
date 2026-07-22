---
api_key_in: []
auth_types:
- http-bearer
- oidc-exchange
description: ''
kind: authentication
layout: security
method: searched
name: Vlt Authentication
name_suffix: Authentication
oauth_flows: []
overview: vlt secures its APIs with http-bearer and oidc-exchange across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: vlt
provider_slug: vlt
scheme_count: 4
schemes:
- description: vlt login performs the npm web login flow against any registry that supports it (including the default registry), storing the resulting token in the local keychain. vlt logout removes the local token and attempts to destroy it server-side.
  name: npm-web-login
  scheme: bearer
  type: http
- description: Registries that issue bearer tokens are supported via vlt token add (stored in vlt's keychain) or the VLT_TOKEN environment variable for CI/headless use. Per-registry tokens use VLT_TOKEN_{registry-url-with-non- alphanumerics-replaced-by-underscores}.
  name: bearer-token
  scheme: bearer
  type: http
- description: OIDC trusted publishing - in supported CI providers vlt requests an OIDC ID token and exchanges it with the registry's token endpoint for a short-lived publish credential; nothing persists after the job. Native support for GitHub Actions (id-token write permission + vltpkg/setup-vlt); GitLab CI and CircleCI via the NPM_ID_TOKEN environment variable. Falls back silently to VLT_TOKEN or keychain auth when OIDC is unavailable.
  name: ci-oidc-exchange
  type: openIdConnect
- description: One-time password (OTP) / MFA is supported on registries that require it.
  name: otp-mfa
  scheme: bearer
  type: http
slug: vlt-authentication
source_filename: vlt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://docs.vlt.io/cli/auth\nsource: https://docs.vlt.io/cli/auth\nnotes: No public OpenAPI is published for the hosted registry (registry.vlt.io\n  is authentication-gated end to end, including /-/ping), so this profile is\n  captured from the published authentication documentation rather than derived\n  from a spec. Self-hosted vsr instances serve their own OpenAPI at /-/api.\nsummary:\n  types: [http-bearer, oidc-exchange]\n  flows: [npm-web-login, bearer-token, env-token, ci-oidc-exchange]\n  mfa: true\nschemes:\n- name: npm-web-login\n  type: http\n  scheme: bearer\n  description: vlt login performs the npm web login flow against any registry\n    that supports it (including the default registry), storing the resulting\n    token in the local keychain. vlt logout removes the local token and\n    attempts to destroy it server-side.\n- name: bearer-token\n  type: http\n  scheme: bearer\n  description: Registries that issue\
  \ bearer tokens are supported via vlt token\n    add (stored in vlt's keychain) or the VLT_TOKEN environment variable for\n    CI/headless use. Per-registry tokens use VLT_TOKEN_{registry-url-with-non-\n    alphanumerics-replaced-by-underscores}.\n- name: ci-oidc-exchange\n  type: openIdConnect\n  description: OIDC trusted publishing - in supported CI providers vlt requests\n    an OIDC ID token and exchanges it with the registry's token endpoint for a\n    short-lived publish credential; nothing persists after the job. Native\n    support for GitHub Actions (id-token write permission + vltpkg/setup-vlt);\n    GitLab CI and CircleCI via the NPM_ID_TOKEN environment variable. Falls\n    back silently to VLT_TOKEN or keychain auth when OIDC is unavailable.\n- name: otp-mfa\n  type: http\n  scheme: bearer\n  description: One-time password (OTP) / MFA is supported on registries that\n    require it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vlt/refs/heads/main/authentication/vlt-authentication.yml
summary_line: http-bearer/oidc-exchange · 4 schemes
tags:
- Company
- JavaScript
- Package Management
- Package Registry
- Developer Tools
- CLI
- Serverless
- npm
- Dependency Management
- Open Source
---
