---
api_key_in:
- header
api_specs:
- filename: veeva-authentication-api-openapi.yml
  format: yaml
  label: veeva Authentication API
  slug: veeva-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-authentication-api-openapi.yml
- filename: veeva-documents-api-openapi.yml
  format: yaml
  label: veeva Documents API
  slug: veeva-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-documents-api-openapi.yml
- filename: veeva-objects-api-openapi.yml
  format: yaml
  label: veeva Objects API
  slug: veeva-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-objects-api-openapi.yml
- filename: veeva-query-api-openapi.yml
  format: yaml
  label: veeva Query API
  slug: veeva-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-query-api-openapi.yml
- filename: veeva-users-api-openapi.yml
  format: yaml
  label: veeva Users API
  slug: veeva-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-users-api-openapi.yml
- filename: veeva-workflows-api-openapi.yml
  format: yaml
  label: veeva Workflows API
  slug: veeva-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-workflows-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Veeva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veeva secures its APIs with apiKey, http, oauth2, and openIdConnect across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Veeva
provider_slug: veeva
scheme_count: 6
schemes:
- description: Vault session ID returned by POST /api/{version}/auth, sent raw in the Authorization header (no Bearer prefix). Idles out after 20 minutes of inactivity; Session Keep Alive extends it, End Session revokes it.
  docs: https://general.veevavault.dev/vault-api/explanation/session-management
  in: header
  name: VaultSession
  parameter: Authorization
  sources:
  - openapi/veeva-authentication-api-openapi.yml
  - https://general.veevavault.dev/vault-api/api-reference/26.2/authentication/user-name-and-password
  type: apiKey
- description: Long-lived API access token generated from the user profile in the Vault UI or via the API Access Token endpoints. Scoped to a single Vault; grants API access only, never UI access. Optional expiry date. Up to 25 active tokens per user. The value is shown once at creation and cannot be recovered. This is the credential the Vault MCP Server requires.
  docs: https://general.veevavault.dev/vault-api/explanation/api-access-tokens
  in: header
  lifecycle:
    created_by:
    - Vault UI user profile
    - POST API Access Token endpoints
    - Generate API Access Token for Sandbox
    queryable_as: api_access_token__sys (VQL / Retrieve Object Record)
    revoked_by: Delete Object Records against api_access_token__sys, or from the user profile page.
    sandbox_behaviour: Not copied into a newly created sandbox (regenerate); copied on sandbox refresh; not copied when promoting a pre-production Vault to production; deleted when a user converts to VeevaID.
  name: ApiAccessToken
  parameter: Authorization
  prefix: Bearer veeva-vault-
  scheme: bearer
  type: http
- description: 'Present an access token issued by the customer''s authorization server as `Authorization: Bearer <access_token>`; Vault validates it via the authorization server''s introspection endpoint (optionally matching the supplied client_id) and returns a Vault session ID. Body accepts optional vaultDNS and client_id.'
  docs: https://general.veevavault.dev/vault-api/api-reference/26.2/authentication/oauth-20-openid-connect
  flow: token-exchange
  method: POST
  name: OAuth2OIDC
  scopes_note: Vault publishes no OAuth scope vocabulary. Authorization is enforced by Vault permission sets and security profiles, not by token scopes, so there is no scopes/ artifact to write.
  scopes_published: false
  token_endpoint: https://login.veevavault.com/auth/oauth/session/{oauth_oidc_profile_id}
  type: oauth2
- description: SAML/SSO delegated authentication; exempt from the Auth API burst limit.
  docs: https://general.veevavault.dev/vault-api/api-reference/26.2/authentication
  name: SAML-SSO
  type: openIdConnect
- description: Initiate a delegated session to act within another user's Vault where a delegation has been granted. Retrieve Delegations lists what the caller may delegate into.
  docs: https://general.veevavault.dev/vault-api/api-reference/26.2/authentication/delegated-access
  in: header
  name: DelegatedAccess
  parameter: Authorization
  type: apiKey
- description: Salesforce-delegated requests for Veeva CRM / Salesforce-integrated flows.
  docs: https://general.veevavault.dev/vault-api/api-reference/26.2/authentication/salesforcetrade-delegated-requests
  in: header
  name: SalesforceDelegated
  parameter: Authorization
  type: apiKey
slug: veeva-authentication
source_filename: veeva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: https://general.veevavault.dev/vault-api/getting-started/authenticating\ndocs: https://general.veevavault.dev/vault-api/api-reference/26.2/authentication\nsummary:\n  types: [apiKey, http, oauth2, openIdConnect]\n  api_key_in: [header]\n  bearer: true\n  oauth2_flow: token-exchange (external IdP access token -> Vault session ID)\n  mfa: Delegated to the configured SAML/SSO or OAuth2/OIDC identity provider.\nschemes:\n  - name: VaultSession\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: >-\n      Vault session ID returned by POST /api/{version}/auth, sent raw in the Authorization\n      header (no Bearer prefix). Idles out after 20 minutes of inactivity; Session Keep Alive\n      extends it, End Session revokes it.\n    docs: https://general.veevavault.dev/vault-api/explanation/session-management\n    sources: [openapi/veeva-authentication-api-openapi.yml, https://general.veevavault.dev/vault-api/api-reference/26.2/authentication/user-name-and-password]\n\
  \  - name: ApiAccessToken\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    prefix: 'Bearer veeva-vault-'\n    description: >-\n      Long-lived API access token generated from the user profile in the Vault UI or via the\n      API Access Token endpoints. Scoped to a single Vault; grants API access only, never UI\n      access. Optional expiry date. Up to 25 active tokens per user. The value is shown once\n      at creation and cannot be recovered. This is the credential the Vault MCP Server requires.\n    docs: https://general.veevavault.dev/vault-api/explanation/api-access-tokens\n    lifecycle:\n      created_by: [Vault UI user profile, POST API Access Token endpoints, Generate API Access Token for Sandbox]\n      revoked_by: Delete Object Records against api_access_token__sys, or from the user profile page.\n      queryable_as: api_access_token__sys (VQL / Retrieve Object Record)\n      sandbox_behaviour: >-\n        Not copied into a newly created\
  \ sandbox (regenerate); copied on sandbox refresh; not\n        copied when promoting a pre-production Vault to production; deleted when a user converts to VeevaID.\n  - name: OAuth2OIDC\n    type: oauth2\n    flow: token-exchange\n    token_endpoint: https://login.veevavault.com/auth/oauth/session/{oauth_oidc_profile_id}\n    method: POST\n    description: >-\n      Present an access token issued by the customer's authorization server as\n      `Authorization: Bearer <access_token>`; Vault validates it via the authorization server's\n      introspection endpoint (optionally matching the supplied client_id) and returns a Vault\n      session ID. Body accepts optional vaultDNS and client_id.\n    scopes_published: false\n    scopes_note: >-\n      Vault publishes no OAuth scope vocabulary. Authorization is enforced by Vault permission\n      sets and security profiles, not by token scopes, so there is no scopes/ artifact to write.\n    docs: https://general.veevavault.dev/vault-api/api-reference/26.2/authentication/oauth-20-openid-connect\n\
  \  - name: SAML-SSO\n    type: openIdConnect\n    description: SAML/SSO delegated authentication; exempt from the Auth API burst limit.\n    docs: https://general.veevavault.dev/vault-api/api-reference/26.2/authentication\n  - name: DelegatedAccess\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: >-\n      Initiate a delegated session to act within another user's Vault where a delegation has\n      been granted. Retrieve Delegations lists what the caller may delegate into.\n    docs: https://general.veevavault.dev/vault-api/api-reference/26.2/authentication/delegated-access\n  - name: SalesforceDelegated\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: Salesforce-delegated requests for Veeva CRM / Salesforce-integrated flows.\n    docs: https://general.veevavault.dev/vault-api/api-reference/26.2/authentication/salesforcetrade-delegated-requests\ndiscovery:\n  - {name: Authentication Type Discovery, detail: Returns which\
  \ authentication types a given user or Vault supports.}\n  - {name: Retrieve API Versions, detail: Lists the API versions available on the Vault.}\n  - {name: Validate Session User, detail: Confirms the session is valid and identifies the user.}\nnotes:\n  - Authentication version need not match the version used for subsequent calls (auth on v17.3, run on v26.2).\n  - >-\n    Auth calls are rate limited separately on username + vaultDNS; exceeding the Auth burst\n    limit FAILS requests rather than delaying them. SAML/SSO and OAuth authentication are\n    exempt from that limit. See rate-limits/veeva-rate-limits.yml.\n  - The Vault MCP Server accepts ONLY the Bearer API access token — not OAuth 2.0 and not basic auth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/authentication/veeva-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 6 schemes
tags:
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- Regulatory
- Quality Management
- Document-Management
- Content Management
- Healthcare
- Software-as-a-Service
- Enterprise
- MCP
- Agents
---
