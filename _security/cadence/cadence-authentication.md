---
anonymous_access: false
api_key_in: []
auth_types: []
description: How a client authenticates to the callable API surfaces Cadence Design Systems operates. There is no OpenAPI to derive securitySchemes from — no machine readable contract is published for any Cadence surface (see conformance/cadence-conformance.yml) — so this profile is read from the provider's own developer documentation and from a live unauthenticated probe of the MMDS API.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Cadence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cadence Design Systems declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Cadence Design Systems
provider_slug: cadence
scheme_count: 4
schemes:
- description: Orion clients (the orionclient Python library and the `ocli` CLI) authenticate with an account token. A profile is a tuple of Orion domain, username, token and project, stored locally by `ocli config profile`; the OCLI config directory and file permissions are forced to read/write for the owner only.
  docs: https://docs.eyesopen.com/orion-developer/modules/orion-platform/docs/orionclient/cli.html
  host: orion.eyesopen.com
  id: orion-api-token
  in: client-managed
  multi_tenant_note: Orion 2026.4 release notes state that OCLI for multitenant customers is available to licensed users according to permissions defined by new roles.
  surface: Orion Molecular Design Platform API
  token_issuance: '"Tokens can be created by logging into Orion with a web browser, going to the user profile, and clicking Create Token under My Tokens." Tokens are also managed from the CLI with `ocli tokens create|list|info|update|delete`.'
  token_lifecycle:
    create: ocli tokens create <description>
    list: ocli tokens list — does not display the value associated with the tokens
    revoke: ocli tokens delete <id>
    rotate: ocli tokens update <id> changes the description only; rotation is create-new + delete-old
  type: apiKey
  verified: Documented, not probed — Orion's API is behind the tenant stack and no anonymous endpoint was found to observe the header form.
- base_url: https://mmds.eyesopen.com/api/v1/
  description: MMDSSessionConfig takes token, user, password, protocol, domain, orion_credentials and api_prefix; the documented pattern inside an Orion cube passes the Orion API token as `orion_credentials` together with the Orion username, so MMDS delegates to the same Orion account token.
  docs: https://docs.eyesopen.com/webservices/mmds/quickstart.html
  host: mmds.eyesopen.com
  id: mmds-orion-credentials
  in: session
  probe:
    allow_header: GET, HEAD, OPTIONS
    body: '{"detail":"Authentication credentials were not provided."}'
    http_status: 403
    note: A live unauthenticated request returns a Django REST Framework 403 with a JSON detail body — the API is real and reachable, and every path is authentication-gated. No WWW-Authenticate challenge is emitted, so the exact header form cannot be established anonymously and is NOT recorded here rather than guessed.
    observed: '2026-09-05'
    url: https://mmds.eyesopen.com/api/v1/auth/
  surface: MMDS — Macromolecular Data Service REST API
  type: apiKey
  verified: probed
- description: The Glyph client connects to a Glyph Server exposed by a running Pointwise /Fidelity session rather than to a hosted HTTP API; access is controlled by the licensed desktop session, not by an issued API credential.
  docs: https://github.com/pointwise/GlyphClientPython
  id: pointwise-glyph-server
  surface: Fidelity Pointwise Glyph Server
  type: local-socket
  verified: searched
- description: Cadence Online Support runs on Salesforce Experience Cloud and publishes a full OpenID Connect discovery document anonymously — authorization, token, userinfo, revocation, introspection, dynamic registration and end-session endpoints, a JWKS URI, 36 supported scopes and 24 supported claims. This is the one machine-readable authentication document anywhere in the Cadence estate.
  discovery: https://support.cadence.com/.well-known/openid-configuration
  dpop_supported: true
  dynamic_client_registration: true
  grants:
  - authorization_code
  - implicit
  host: support.cadence.com
  id: cadence-support-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://support.cadence.com
  note: This authenticates users and clients into the Cadence support portal. It is NOT the auth model for the Orion or MMDS APIs, which use account tokens.
  probe:
    content_type: application/json
    http_status: 200
    observed: '2026-09-05'
    url: https://support.cadence.com/.well-known/openid-configuration
  saved_document: well-known/cadence-support-openid-configuration.json
  scopes: scopes/cadence-scopes.yml
  surface: Cadence Online Support portal (support.cadence.com)
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
  verified: probed
slug: cadence-authentication
source_filename: cadence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://docs.eyesopen.com/orion-developer/modules/orion-platform/docs/orionclient/cli.html ·\n  https://docs.eyesopen.com/webservices/mmds/client.html ·\n  https://docs.eyesopen.com/webservices/mmds/quickstart.html\ndescription: >-\n  How a client authenticates to the callable API surfaces Cadence Design Systems\n  operates. There is no OpenAPI to derive securitySchemes from — no machine\n  readable contract is published for any Cadence surface (see\n  conformance/cadence-conformance.yml) — so this profile is read from the\n  provider's own developer documentation and from a live unauthenticated probe\n  of the MMDS API.\ndocs: https://docs.eyesopen.com/orion-developer/index.html\n\nschemes:\n  - id: orion-api-token\n    type: apiKey\n    surface: Orion Molecular Design Platform API\n    host: orion.eyesopen.com\n    in: client-managed\n    description: >-\n      Orion clients (the orionclient Python library and the `ocli`\
  \ CLI)\n      authenticate with an account token. A profile is a tuple of Orion domain,\n      username, token and project, stored locally by `ocli config profile`; the\n      OCLI config directory and file permissions are forced to read/write for\n      the owner only.\n    token_issuance: >-\n      \"Tokens can be created by logging into Orion with a web browser, going to\n      the user profile, and clicking Create Token under My Tokens.\" Tokens are\n      also managed from the CLI with `ocli tokens create|list|info|update|delete`.\n    token_lifecycle:\n      create: ocli tokens create <description>\n      list: \"ocli tokens list — does not display the value associated with the tokens\"\n      rotate: \"ocli tokens update <id> changes the description only; rotation is create-new + delete-old\"\n      revoke: ocli tokens delete <id>\n    multi_tenant_note: >-\n      Orion 2026.4 release notes state that OCLI for multitenant customers is\n      available to licensed users according\
  \ to permissions defined by new roles.\n    docs: https://docs.eyesopen.com/orion-developer/modules/orion-platform/docs/orionclient/cli.html\n    verified: >-\n      Documented, not probed — Orion's API is behind the tenant stack and no\n      anonymous endpoint was found to observe the header form.\n\n  - id: mmds-orion-credentials\n    type: apiKey\n    surface: MMDS — Macromolecular Data Service REST API\n    host: mmds.eyesopen.com\n    base_url: https://mmds.eyesopen.com/api/v1/\n    in: session\n    description: >-\n      MMDSSessionConfig takes token, user, password, protocol, domain,\n      orion_credentials and api_prefix; the documented pattern inside an Orion\n      cube passes the Orion API token as `orion_credentials` together with the\n      Orion username, so MMDS delegates to the same Orion account token.\n    probe:\n      url: https://mmds.eyesopen.com/api/v1/auth/\n      http_status: 403\n      body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n\
  \      allow_header: GET, HEAD, OPTIONS\n      observed: '2026-09-05'\n      note: >-\n        A live unauthenticated request returns a Django REST Framework 403 with a\n        JSON detail body — the API is real and reachable, and every path is\n        authentication-gated. No WWW-Authenticate challenge is emitted, so the\n        exact header form cannot be established anonymously and is NOT recorded\n        here rather than guessed.\n    docs: https://docs.eyesopen.com/webservices/mmds/quickstart.html\n    verified: probed\n\n  - id: pointwise-glyph-server\n    type: local-socket\n    surface: Fidelity Pointwise Glyph Server\n    description: >-\n      The Glyph client connects to a Glyph Server exposed by a running Pointwise\n      /Fidelity session rather than to a hosted HTTP API; access is controlled by\n      the licensed desktop session, not by an issued API credential.\n    docs: https://github.com/pointwise/GlyphClientPython\n    verified: searched\n\n  - id: cadence-support-oidc\n\
  \    type: openIdConnect\n    surface: Cadence Online Support portal (support.cadence.com)\n    host: support.cadence.com\n    issuer: https://support.cadence.com\n    discovery: https://support.cadence.com/.well-known/openid-configuration\n    saved_document: well-known/cadence-support-openid-configuration.json\n    description: >-\n      Cadence Online Support runs on Salesforce Experience Cloud and publishes a\n      full OpenID Connect discovery document anonymously — authorization, token,\n      userinfo, revocation, introspection, dynamic registration and end-session\n      endpoints, a JWKS URI, 36 supported scopes and 24 supported claims. This\n      is the one machine-readable authentication document anywhere in the\n      Cadence estate.\n    grants: [authorization_code, implicit]\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic, private_key_jwt]\n    id_token_signing_alg: [RS256]\n    dpop_supported: true\n    dynamic_client_registration: true\n   \
  \ scopes: scopes/cadence-scopes.yml\n    probe: {url: 'https://support.cadence.com/.well-known/openid-configuration', http_status: 200, content_type: application/json, observed: '2026-09-05'}\n    verified: probed\n    note: >-\n      This authenticates users and clients into the Cadence support portal. It is\n      NOT the auth model for the Orion or MMDS APIs, which use account tokens.\n\noauth2: true\nopenid_connect: true\nmutual_tls: false\nscopes_surface: >-\n  Published only by the support portal's OIDC discovery document (36 Salesforce\n  platform scopes — see scopes/cadence-scopes.yml). The Orion and MMDS APIs have\n  no scope model: Orion authorisation is expressed as project/workspace/\n  organization sharing and, since 2026.4, as multitenant roles.\n\ngaps:\n  - No public OpenAPI or securitySchemes block exists for any Cadence surface.\n  - No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on ANY eyesopen host, nor on the cadence.com edge (404 or\
  \ Cloudflare-challenged on 2026-09-05). The only discovery document in the estate is the support-portal one recorded above; see well-known/cadence-well-known.yml.\n  - Cadence's EDA products (Virtuoso, Allegro X, OrCAD X, Xcelium) are licence-managed desktop/compute software and publish no API credential model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cadence/refs/heads/main/authentication/cadence-authentication.yml
summary_line: 4 schemes
tags:
- Electronic Design Automation
- EDA
- Semiconductors
- Chip Design
- IC Design
- PCB Design
- Software
- Company
---
