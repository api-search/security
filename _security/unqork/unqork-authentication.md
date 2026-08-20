---
api_key_in: []
api_specs:
- filename: unqork-customer-api-openapi.yml
  format: yaml
  label: Unqork Customer API
  slug: unqork-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unqork/refs/heads/main/openapi/unqork-customer-api-openapi.yml
auth_types:
- oauth2
description: The Unqork Customer API authenticates exclusively with OAuth 2.0 bearer tokens. Two grants are supported — client credentials (the default and recommended path) and the resource-owner password grant (off by default, enabled per environment). There are no API keys and no basic-auth path to the resources themselves; HTTP Basic is used only to present client credentials at the token endpoint. Authorization is RBAC, not scopes.
kind: authentication
layout: security
method: searched
name: Unqork Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Unqork secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Unqork
provider_slug: unqork
scheme_count: 1
schemes:
- applied: 'Document-level `security: [{OAuth2: []}]` — every one of the 93 operations requires a bearer token.'
  description: 'The Unqork API implements the OAuth 2.0 Client Credentials Grant and the OAuth 2.0 Password Grant. Client credentials are created on the API Access Management administration page. The token endpoint returns an access_token which expires after one hour, after which a new one must be retrieved. The token is presented on every request as an Authorization: Bearer header.'
  flows:
  - credential_source: Administration → API Access Management
    flow: clientCredentials
    recommended: true
    request: curl -u '{clientId}:{clientSecret}' -X POST --basic https://{subdomain}.unqork.io/api/1.0/oauth2/access_token -d "grant_type=client_credentials"
    rfc: RFC 6749 §1.3.4
    scopes: 1
    scopes_note: single placeholder scope `none` (N/A) — not a real permission
    spec_tokenUrl: https://xyzfinancial.unqork.io/api/1.0/oauth2/access_token
    tokenUrl: https://{subdomain}.unqork.io/api/1.0/oauth2/access_token
  - caveat: Removed in OAuth 2.1 and discouraged by RFC 9700 (OAuth 2.0 Security Best Current Practice). Enabling it widens the token-issuing surface to every human account in the environment.
    enabled_by_default: false
    enablement: Administration → Environment Administration → Unqork API → "Enable OAuth2 Password Grant". Once enabled, ALL Unqork users in the environment can exchange their platform username/password for an access token.
    flow: password
    recommended: false
    request: curl -X POST https://{subdomain}.unqork.io/api/1.0/oauth2/access_token -d "grant_type=password&username={username}&password={password}"
    rfc: RFC 6749 §1.3.3
    scopes: 1
    spec_tokenUrl: https://xyzfinancial.unqork.io/api/1.0/oauth2/access_token
    tokenUrl: https://{subdomain}.unqork.io/api/1.0/oauth2/access_token
  name: OAuth2
  sources:
  - openapi/unqork-customer-api-openapi.yml
  type: oauth2
slug: unqork-authentication
source_filename: unqork-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: openapi/unqork-customer-api-openapi.yml\ndocs:\n  - https://docs.unqork.io/docs/api-authentication\n  - https://docs.unqork.io/docs/api-access-management\n  - https://docs.unqork.io/docs/api-authentication-bearer-token\n  - https://docs.unqork.io/docs/connect-to-the-unqork-api\ndescription: >-\n  The Unqork Customer API authenticates exclusively with OAuth 2.0 bearer tokens.\n  Two grants are supported — client credentials (the default and recommended\n  path) and the resource-owner password grant (off by default, enabled per\n  environment). There are no API keys and no basic-auth path to the resources\n  themselves; HTTP Basic is used only to present client credentials at the token\n  endpoint. Authorization is RBAC, not scopes.\n\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials, password]\n  api_key_in: []\n  bearer_header: 'Authorization: Bearer {access_token}'\n  token_lifetime_seconds: 3600\n  scope_based:\
  \ false\n  authorization_model: rbac\n  applied_globally: true\n\nschemes:\n  - name: OAuth2\n    type: oauth2\n    applied: >-\n      Document-level `security: [{OAuth2: []}]` — every one of the 93 operations\n      requires a bearer token.\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://{subdomain}.unqork.io/api/1.0/oauth2/access_token\n        spec_tokenUrl: https://xyzfinancial.unqork.io/api/1.0/oauth2/access_token\n        scopes: 1\n        scopes_note: single placeholder scope `none` (N/A) — not a real permission\n        rfc: RFC 6749 §1.3.4\n        recommended: true\n        credential_source: Administration → API Access Management\n        request: >-\n          curl -u '{clientId}:{clientSecret}' -X POST --basic\n          https://{subdomain}.unqork.io/api/1.0/oauth2/access_token\n          -d \"grant_type=client_credentials\"\n      - flow: password\n        tokenUrl: https://{subdomain}.unqork.io/api/1.0/oauth2/access_token\n        spec_tokenUrl:\
  \ https://xyzfinancial.unqork.io/api/1.0/oauth2/access_token\n        scopes: 1\n        rfc: RFC 6749 §1.3.3\n        recommended: false\n        enabled_by_default: false\n        enablement: >-\n          Administration → Environment Administration → Unqork API →\n          \"Enable OAuth2 Password Grant\". Once enabled, ALL Unqork users in the\n          environment can exchange their platform username/password for an\n          access token.\n        caveat: >-\n          Removed in OAuth 2.1 and discouraged by RFC 9700 (OAuth 2.0 Security\n          Best Current Practice). Enabling it widens the token-issuing surface to\n          every human account in the environment.\n        request: >-\n          curl -X POST https://{subdomain}.unqork.io/api/1.0/oauth2/access_token\n          -d \"grant_type=password&username={username}&password={password}\"\n    description: >-\n      The Unqork API implements the OAuth 2.0 Client Credentials Grant and the\n      OAuth 2.0 Password Grant.\
  \ Client credentials are created on the API Access\n      Management administration page. The token endpoint returns an access_token\n      which expires after one hour, after which a new one must be retrieved. The\n      token is presented on every request as an Authorization: Bearer header.\n    sources:\n      - openapi/unqork-customer-api-openapi.yml\n\ncredential_surfaces:\n  - name: Express\n    purpose: End-user-facing API access (submissions, workflow execution) in Express View\n    role_requirement: At least one Express Role is required to create a credential\n    role_admin: https://docs.unqork.io/docs/express-role-administration\n    permissions: https://docs.unqork.io/docs/express-permissions\n    revocable: false\n  - name: Creator\n    purpose: Design-time API access (modules, applications, promotions, credentials)\n    role_requirement: At least one Creator Role is required to create a credential\n    role_admin: https://docs.unqork.io/docs/creator-role-administration\n\
  \    permissions: https://docs.unqork.io/docs/creator-permissions\n    revocable: true\n\ncredential_lifecycle:\n  client_id_prefix: uq\n  client_id_example_shape: uq + 24 hex characters\n  secret_visibility: >-\n    The Client Secret is displayed exactly once, in the Client ID & Secret modal\n    at creation time, and is not retrievable afterwards. If lost, an administrator\n    must generate a new secret (the Client ID is retained).\n  expiration_days: {min: 1, max: 730, ui_default: 90}\n  statuses:\n    ACTIVE: Currently active and able to access the API\n    EXPIRES SOON: Set when 15% or less of the validity window remains (14 days on a 90-day credential)\n    EXPIRED: Past the expiration date; can no longer access the APIs\n    REVOKED: Administrator has removed API access (Creator credentials only)\n    LOCKED: >-\n      Temporarily disabled after up to five failed client-secret login attempts;\n      automatically reverts to ACTIVE after 30 minutes\n  managed_via_api:\n    list:\
  \ credentialsGetAll\n    create: credentialsCreate\n    update: credentialsUpdate\n    revoke: credentialsRevoke\n    delete: credentialsDeleteById\n  delete_is_permanent: true\n\nadditional_mechanisms:\n  - name: Referstring\n    operation: generateReferString\n    path: POST /referstring\n    description: Generates an encrypted referstring for authentication.\n    note: Mints authentication material — handle like a secret.\n  - name: mTLS with OAuth 2.0\n    direction: outbound\n    description: >-\n      Client mutual-TLS certificates can be paired with OAuth 2.0 for OUTBOUND\n      integrations from Unqork modules to external services. This is not an\n      inbound securityScheme on the Customer API.\n    docs: https://docs.unqork.io/docs/how-to-setup-an-mtls-certificate-with-oauth-20-authentication\n  - name: SAML SSO\n    scope: platform login, not the Customer API\n    description: >-\n      Unqork supports SAML single sign-on for platform and community access\n      (the Community\
  \ Hub exposes an ssoType=saml proxy). The Customer API itself\n      is OAuth 2.0 only.\n  - name: PIV/CAC\n    scope: US Government customers\n    description: >-\n      PIV/CAC authentication is offered for US Government deployments as part of\n      Unqork's FedRAMP posture.\n    source: https://unqork.com/security-compliance/\n\nanonymous_access:\n  supported: true\n  context: webhook receivers only\n  note: >-\n    A module configured to receive external webhooks must grant anonymous-user\n    RBAC permissions, which makes its URL publicly callable with no\n    authentication and no signature verification. See asyncapi/unqork-webhooks.yml.\n\ndiscovery:\n  openid_configuration: false\n  oauth_authorization_server_metadata: false\n  note: >-\n    Neither /.well-known/openid-configuration nor\n    /.well-known/oauth-authorization-server (RFC 8414) is served on any Unqork\n    host — see well-known/unqork-well-known.yml. Token endpoint and grant support\n    are documented only in prose\
  \ and in the OpenAPI securityScheme description.\n\ngaps:\n  - No RFC 8414 authorization-server metadata document.\n  - No OIDC / openIdConnect scheme.\n  - No refresh-token flow documented — a one-hour token must be re-minted from credentials.\n  - No scopes, so no way to request a read-only token.\n  - >-\n    No PKCE / authorization-code flow, so there is no delegated-user\n    authorization path for third-party applications.\n\nrelated:\n  scopes: scopes/unqork-scopes.yml\n  conventions: conventions/unqork-conventions.yml\n  lifecycle: lifecycle/unqork-lifecycle.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unqork/refs/heads/main/authentication/unqork-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- No-Code
- Low-Code
- Application Development
- Enterprise Software
- Platform-as-a-Service
- Workflows
- Financial-Services
- Insurance
- Government
- Application Modernization
---
