---
api_key_in: []
auth_types: []
description: 'Tailor separates two authentication planes. The PLATFORM plane (api.tailor.tech) authenticates operators and tooling against the control-plane API with OAuth 2.0 or a personal access token. The APPLICATION plane is provisioned per customer: each Tailor application configures its own Auth service, its own OAuth2 clients, and optionally an external IdP over OIDC or SAML.'
kind: authentication
layout: security
method: searched
name: Tailor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tailor declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Tailor
provider_slug: tailor
scheme_count: 0
schemes: []
slug: tailor-authentication
source_filename: tailor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://docs.tailor.tech/guides/auth/overview\ndocs: https://docs.tailor.tech/guides/auth/overview\nname: Tailor authentication profile\ndescription: >-\n  Tailor separates two authentication planes. The PLATFORM plane (api.tailor.tech)\n  authenticates operators and tooling against the control-plane API with OAuth 2.0 or a\n  personal access token. The APPLICATION plane is provisioned per customer: each Tailor\n  application configures its own Auth service, its own OAuth2 clients, and optionally an\n  external IdP over OIDC or SAML.\nplanes:\n- name: platform\n  host: api.tailor.tech\n  issuer: https://api.tailor.tech\n  discovery: https://api.tailor.tech/.well-known/oauth-authorization-server\n  discovery_status: 200\n  metadata_file: well-known/tailor-oauth-authorization-server.json\n  schemes:\n  - type: oauth2\n    id: platform_oauth2\n    flows:\n      authorization_code:\n        authorizationUrl: https://api.tailor.tech/oauth2/platform/authorize\n\
  \        tokenUrl: https://api.tailor.tech/oauth2/platform/token\n        pkce: required\n        pkce_methods: [S256]\n      client_credentials:\n        tokenUrl: https://api.tailor.tech/oauth2/platform/token\n      refresh_token:\n        tokenUrl: https://api.tailor.tech/oauth2/platform/token\n    revocation_endpoint: https://api.tailor.tech/oauth2/platform/revoke\n    userinfo_endpoint: https://api.tailor.tech/oauth2/platform/userinfo\n    token_endpoint_auth_methods:\n    - client_secret_basic\n    - client_secret_post\n    - none\n    dpop:\n      supported: true\n      bound_access_tokens: false\n      nonce_supported: true\n      signing_algs: [ES256, RS256]\n  - type: http\n    scheme: bearer\n    id: personal_access_token\n    token_prefix: tpp_\n    description: >-\n      Personal Access Token. Created with `tailor user pat create <name>` (or\n      `npx @tailor-platform/tailor-mcp auth pat create --name mcp --scopes write --scopes read`)\n      and supplied as a Bearer token,\
  \ or via the TAILOR_TOKEN environment variable for\n      MCP clients that cannot use the stored credential file.\n    scopes: [read, write]\n- name: application\n  host: per-workspace, provisioned by Tailor\n  description: >-\n    Configured in code with `defineAuth()`. Each application declares its own\n    oauth2Clients (redirectURIs, grantTypes), a userProfile mapped onto a TailorDB type,\n    machineUsers for service accounts, and an optional external identity provider.\n  schemes:\n  - type: oauth2\n    id: application_oauth2\n    description: Application-declared OAuth2 clients; grant types are chosen per client (authorization_code, refresh_token).\n    pkce: supported (DPoP + PKCE via @tailor-platform/auth-public-client)\n  - type: openIdConnect\n    id: external_idp_oidc\n    description: SSO against an external identity provider over OIDC.\n  - type: saml\n    id: external_idp_saml\n    description: SSO against an external identity provider over SAML.\n  - type: http\n    scheme:\
  \ bearer\n    id: machine_user\n    description: Service accounts (\"machine users\") for automated processes and API access.\n  features:\n  - Built-in IdP (Preview) — Tailor can act as the identity provider itself\n  - Auth Hooks — custom logic at the BEFORE_LOGIN hook point\n  - SCIM provisioning — AuthSCIMConfig/AuthSCIMResource, bearer or OAuth2 authorized\n  - Subgraph integration — user records queryable directly through the application GraphQL API\naccess_control:\n  model: role- and attribute-based\n  description: >-\n    Users are mapped to a TailorDB type with attributes (for example a role enum), and\n    access to resources is controlled from those roles and attributes. IP allowlists\n    (CIDR) can be applied at organization, folder, or application level and are enforced\n    at the routing layer before a request reaches an application.\ntransport_security:\n  tls_required: true\n  encryption_at_rest: AES-256\n  encryption_in_transit: TLS\n  source: https://docs.tailor.tech/reference/security\n\
  x-evidence:\n  fetched: '2026-08-29'\n  probes:\n  - url: https://api.tailor.tech/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://docs.tailor.tech/guides/auth/overview.md\n    status: 200\n  - url: https://docs.tailor.tech/reference/api/api-references.md\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailor/refs/heads/main/authentication/tailor-authentication.yml
summary_line: 0 schemes
tags:
- Company
- ERP
- Headless ERP
- Retail
- E-Commerce
- Supply Chain
- Inventory Management
- GraphQL
- gRPC
- Low-Code
- Composable Commerce
- Manufacturing
---
