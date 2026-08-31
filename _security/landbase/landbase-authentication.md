---
api_key_in: []
auth_types: []
description: Landbase runs two authentication models side by side, and which one you get depends on a mode switch rather than a per-credential choice. Platform mode (the default) is a browser OAuth consent flow that mints a short-lived session token; legacy mode is a long-lived API key that bypasses the gateway entirely and speaks to the AgentOS backend directly. Both are documented for the CLI. No OpenAPI securitySchemes exist to derive from — this profile is read from the provider's own auth pages and from the one machine-readable artifact on the estate, the OIDC discovery document.
kind: authentication
layout: security
method: searched
name: Landbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Landbase declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Landbase
provider_slug: landbase
scheme_count: 2
schemes:
- default: true
  flow: Browser authorization-code style consent. `landbase-cli auth login` opens a consent page; if the caller is not signed in they are sent to https://gtm.landbase.com to sign in or create an account, then approve the CLI access request. In a headless or SSH environment the CLI prints the URL to stderr instead of opening a browser.
  id: platform-oauth-session
  name: Platform session (OAuth)
  reauth: landbase-cli auth login --force
  routed_through: https://api.landbase.com (the cloud gateway)
  scopes_note: The consent page grants "CLI access" as a single undifferentiated approval. Landbase publishes no scope or permission reference, no scope strings appear anywhere in the documentation, and there is no /.well-known/oauth-authorization-server (404) to read them from — so no scopes/ artifact could be derived. An agent cannot request or verify least privilege.
  scopes_published: false
  stored_at: ~/.landbase/platform.json (mode 0600)
  stored_fields:
  - accessToken
  - expiresAt
  - accountId
  - deviceName
  token_prefix: lbs_
  token_ttl: 7 days — stated in the contacts-import error table ("The platform session expired (7-day TTL) — re-login"). The stored session also carries an explicit expiresAt.
  type: oauth2
- created_by: landbase-cli auth login --key
  default: false
  enable_with: LANDBASE_LEGACY_MODE=1
  env_precedence: LANDBASE_API_KEY wins over the key stored in config.json.
  env_var: LANDBASE_API_KEY
  id: legacy-api-key
  intended_use: Backward compatibility and non-interactive/CI use. The FAQ recommends the API key for CI, scripts and remote servers because the OAuth flow needs a browser.
  key_prefix: lbk_
  name: Legacy API key
  rotation: Documented as safe to edit the apiKey field in config.json directly to rotate a key without re-running auth login. No expiry is stated — these are described as long-lived.
  routed_through: AgentOS backend directly, bypassing the api.landbase.com gateway
  status: legacy — Landbase tells new users to stay on platform mode.
  stored_at: ~/.landbase/config.json (mode 0600, field apiKey)
  type: apiKey
slug: landbase-authentication
source_filename: landbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: >-\n  https://www.landbase.com/docs/reference/auth,\n  https://www.landbase.com/docs/explanation/platform-vs-legacy,\n  https://www.landbase.com/docs/reference/config-files,\n  https://www.landbase.com/docs/reference/env-vars,\n  https://www.landbase.com/docs/how-to/troubleshoot-auth, plus the OIDC discovery document probed at\n  https://api.landbase.com/.well-known/openid-configuration.\ndescription: >-\n  Landbase runs two authentication models side by side, and which one you get depends on a mode\n  switch rather than a per-credential choice. Platform mode (the default) is a browser OAuth consent\n  flow that mints a short-lived session token; legacy mode is a long-lived API key that bypasses the\n  gateway entirely and speaks to the AgentOS backend directly. Both are documented for the CLI. No\n  OpenAPI securitySchemes exist to derive from — this profile is read from the provider's own auth\n  pages and from the one machine-readable\
  \ artifact on the estate, the OIDC discovery document.\nbase_url: https://api.landbase.com\ndocs: https://www.landbase.com/docs/reference/auth\nschemes:\n  - id: platform-oauth-session\n    type: oauth2\n    default: true\n    name: Platform session (OAuth)\n    flow: >-\n      Browser authorization-code style consent. `landbase-cli auth login` opens a consent page; if\n      the caller is not signed in they are sent to https://gtm.landbase.com to sign in or create an\n      account, then approve the CLI access request. In a headless or SSH environment the CLI prints\n      the URL to stderr instead of opening a browser.\n    token_prefix: lbs_\n    token_ttl: >-\n      7 days — stated in the contacts-import error table (\"The platform session expired (7-day TTL)\n      — re-login\"). The stored session also carries an explicit expiresAt.\n    stored_at: ~/.landbase/platform.json (mode 0600)\n    stored_fields: [accessToken, expiresAt, accountId, deviceName]\n    routed_through: https://api.landbase.com\
  \ (the cloud gateway)\n    reauth: landbase-cli auth login --force\n    scopes_published: false\n    scopes_note: >-\n      The consent page grants \"CLI access\" as a single undifferentiated approval. Landbase publishes\n      no scope or permission reference, no scope strings appear anywhere in the documentation, and\n      there is no /.well-known/oauth-authorization-server (404) to read them from — so no\n      scopes/ artifact could be derived. An agent cannot request or verify least privilege.\n  - id: legacy-api-key\n    type: apiKey\n    default: false\n    name: Legacy API key\n    key_prefix: lbk_\n    stored_at: ~/.landbase/config.json (mode 0600, field apiKey)\n    env_var: LANDBASE_API_KEY\n    env_precedence: LANDBASE_API_KEY wins over the key stored in config.json.\n    created_by: landbase-cli auth login --key\n    enable_with: LANDBASE_LEGACY_MODE=1\n    routed_through: AgentOS backend directly, bypassing the api.landbase.com gateway\n    rotation: >-\n      Documented\
  \ as safe to edit the apiKey field in config.json directly to rotate a key without\n      re-running auth login. No expiry is stated — these are described as long-lived.\n    intended_use: >-\n      Backward compatibility and non-interactive/CI use. The FAQ recommends the API key for CI,\n      scripts and remote servers because the OAuth flow needs a browser.\n    status: legacy — Landbase tells new users to stay on platform mode.\noidc:\n  discovery_url: https://api.landbase.com/.well-known/openid-configuration\n  status: 200\n  issuer: platform.landbase.com\n  jwks_uri: /.well-known/jwks.json\n  jwks_status: 200\n  signing_algs: [RS256]\n  key_ids: [platform-jwt-1]\n  conformant: false\n  conformance_note: >-\n    The document is a three-field stub. OpenID Connect Discovery 1.0 requires\n    authorization_endpoint, token_endpoint, response_types_supported and subject_types_supported;\n    none is present, and jwks_uri is a relative path rather than the absolute URL the spec\n    mandates.\
  \ It is enough to verify a platform JWT's signature and nothing else — a relying party\n    cannot drive a login from it. See conformance/landbase-conformance.yml.\ntransport:\n  tls_required: true\n  base_url_allowlist: >-\n    LANDBASE_API_BASE_URL is constrained to *.landbase.com, localhost or 127.0.0.1 unless\n    LANDBASE_ALLOW_CUSTOM_API_URL=1 is set, and the installer applies the same allowlist to\n    LANDBASE_INSTALL_URL. This is a deliberate anti-exfiltration control on a credential-bearing\n    client and is worth crediting.\nerrors:\n  - {code: AUTH_FAILED, exit: 3, meaning: No valid API key or session, or the credentials were rejected.}\n  - {code: AUTH_REQUIRED, exit: 3, meaning: \"Interactive login required (contacts-import surface).\"}\n  - {code: SETUP_FAILED, exit: 1, meaning: A configuration step failed, e.g. a config permissions write.}\ndiagnostics: landbase-cli doctor\ntroubleshooting: https://www.landbase.com/docs/how-to/troubleshoot-auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landbase/refs/heads/main/authentication/landbase-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Go-To-Market
- Sales
- Marketing
- B2B Data
- Data Enrichment
- Artificial Intelligence
- Agents
- Command Line Interface
- Lead Generation
---
