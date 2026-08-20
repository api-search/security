---
api_key_in:
- header
api_specs:
- filename: coresignal-collect-api-openapi.yml
  format: yaml
  label: Coresignal Collect API
  slug: coresignal-collect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/openapi/coresignal-collect-api-openapi.yml
- filename: coresignal-search-api-openapi.yml
  format: yaml
  label: Coresignal Search API
  slug: coresignal-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/openapi/coresignal-search-api-openapi.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Coresignal Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Coresignal secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Coresignal
provider_slug: coresignal
scheme_count: 3
schemes:
- also_issued_by: account manager or sales representative on request for an API plan
  applies_to: All REST endpoints on https://api.coresignal.com/cdapi/v2/
  example_header: 'apikey: <API_Key>'
  expiry: none documented
  format: 32-character alphanumeric string
  in: header
  issued_at: https://dashboard.coresignal.com/ (API keys section)
  multiple_keys: true
  name: apiKey
  note: Entitlement is the plan attached to the account, not the key. Keys can be generated, regenerated and deleted from the dashboard; issuing a key per environment or per downstream tenant is the only isolation mechanism available, since there is no least-privilege model.
  parameter: apikey
  revocable: true
  rotatable: true
  scopes: none
  sources:
  - openapi/_original/coresignal-multi-source-company-api-openapi.yml
  - openapi/_original/coresignal-multi-source-employee-api-openapi.yml
  - openapi/_original/coresignal-multi-source-jobs-api-openapi.yml
  - https://docs.coresignal.com/api-introduction/authorization
  type: apiKey
- applies_to: https://mcp.coresignal.com/mcp/v2 (MCP server)
  bearer_methods_supported:
  - header
  dynamic_client_registration: https://dashboard.coresignal.com/api/auth/oauth2/register
  flows:
  - authorizationUrl: https://dashboard.coresignal.com/api/auth/oauth2/authorize
    flow: authorizationCode
    pkce_required: S256
    scopes:
    - openid
    - profile
    - email
    - offline_access
    tokenUrl: https://dashboard.coresignal.com/api/auth/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://dashboard.coresignal.com/api/auth/oauth2/token
  - flow: refreshToken
    tokenUrl: https://dashboard.coresignal.com/api/auth/oauth2/token
  introspection: https://dashboard.coresignal.com/api/auth/oauth2/introspect
  issuer: https://dashboard.coresignal.com/api/auth
  name: Coresignal Dashboard OAuth 2.1
  note: The MCP server verifies the signed token on each request and retrieves the team's API key server-side, so no key is stored on the server or in client config. Because the protected resource advertises an EMPTY scope list, a valid token grants every tool including the credit-spending ones.
  protected_resource_metadata: https://mcp.coresignal.com/.well-known/oauth-protected-resource/mcp/v2
  resource_scopes_supported: []
  revocation: https://dashboard.coresignal.com/api/auth/oauth2/revoke
  sources:
  - well-known/coresignal-oauth-authorization-server.json
  - well-known/coresignal-oauth-protected-resource.json
  - https://docs.coresignal.com/integrations/coresignal-mcp
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
- acr_values:
  - urn:mace:incommon:iap:bronze
  applies_to: Dashboard sign-in (identity layer under the OAuth 2.1 flow above)
  claims:
  - sub
  - iss
  - aud
  - exp
  - iat
  - sid
  - scope
  - azp
  - email
  - email_verified
  - name
  - picture
  - family_name
  - given_name
  end_session_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/end-session
  id_token_signing_alg:
  - RS256
  jwks_uri: https://dashboard.coresignal.com/api/auth/jwks
  name: Coresignal Dashboard OpenID Connect
  openIdConnectUrl: https://dashboard.coresignal.com/.well-known/openid-configuration
  prompt_values:
  - login
  - consent
  - create
  - select_account
  - none
  sources:
  - well-known/coresignal-openid-configuration.json
  subject_types:
  - public
  type: openIdConnect
  userinfo_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/userinfo
slug: coresignal-authentication
source_filename: coresignal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.coresignal.com/api-introduction/authorization,\n  https://docs.coresignal.com/self-service/account-management/authentication-and-api-keys,\n  https://docs.coresignal.com/integrations/coresignal-mcp,\n  well-known/coresignal-oauth-authorization-server.json,\n  well-known/coresignal-oauth-protected-resource.json,\n  openapi/_original/*.yml\ndocs: https://docs.coresignal.com/api-introduction/authorization\nnote: >-\n  Upgraded from a derived spec-only profile. Coresignal runs TWO distinct authentication models on the\n  same estate and they should not be conflated: the REST data APIs take a bare 32-character API key in\n  an `apikey` header with no scopes and no expiry, while the MCP v2 agent surface takes a full OAuth\n  2.1 authorization-code flow against the dashboard and resolves the team's API key server-side.\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode,\
  \ clientCredentials, refreshToken]\n  oauth2_scope: MCP v2 only\n  mutual_tls: false\n  signed_requests: false\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameter: apikey\n    applies_to: All REST endpoints on https://api.coresignal.com/cdapi/v2/\n    format: 32-character alphanumeric string\n    issued_at: https://dashboard.coresignal.com/ (API keys section)\n    also_issued_by: account manager or sales representative on request for an API plan\n    multiple_keys: true\n    rotatable: true\n    revocable: true\n    expiry: none documented\n    scopes: none\n    note: >-\n      Entitlement is the plan attached to the account, not the key. Keys can be generated, regenerated\n      and deleted from the dashboard; issuing a key per environment or per downstream tenant is the\n      only isolation mechanism available, since there is no least-privilege model.\n    example_header: 'apikey: <API_Key>'\n    sources:\n      - openapi/_original/coresignal-multi-source-company-api-openapi.yml\n\
  \      - openapi/_original/coresignal-multi-source-employee-api-openapi.yml\n      - openapi/_original/coresignal-multi-source-jobs-api-openapi.yml\n      - https://docs.coresignal.com/api-introduction/authorization\n  - name: Coresignal Dashboard OAuth 2.1\n    type: oauth2\n    applies_to: https://mcp.coresignal.com/mcp/v2 (MCP server)\n    issuer: https://dashboard.coresignal.com/api/auth\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://dashboard.coresignal.com/api/auth/oauth2/authorize\n        tokenUrl: https://dashboard.coresignal.com/api/auth/oauth2/token\n        pkce_required: S256\n        scopes: [openid, profile, email, offline_access]\n      - flow: clientCredentials\n        tokenUrl: https://dashboard.coresignal.com/api/auth/oauth2/token\n      - flow: refreshToken\n        tokenUrl: https://dashboard.coresignal.com/api/auth/oauth2/token\n    dynamic_client_registration: https://dashboard.coresignal.com/api/auth/oauth2/register\n    introspection:\
  \ https://dashboard.coresignal.com/api/auth/oauth2/introspect\n    revocation: https://dashboard.coresignal.com/api/auth/oauth2/revoke\n    protected_resource_metadata: https://mcp.coresignal.com/.well-known/oauth-protected-resource/mcp/v2\n    resource_scopes_supported: []\n    bearer_methods_supported: [header]\n    token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n    note: >-\n      The MCP server verifies the signed token on each request and retrieves the team's API key\n      server-side, so no key is stored on the server or in client config. Because the protected\n      resource advertises an EMPTY scope list, a valid token grants every tool including the\n      credit-spending ones.\n    sources:\n      - well-known/coresignal-oauth-authorization-server.json\n      - well-known/coresignal-oauth-protected-resource.json\n      - https://docs.coresignal.com/integrations/coresignal-mcp\n  - name: Coresignal Dashboard OpenID Connect\n    type: openIdConnect\n\
  \    applies_to: Dashboard sign-in (identity layer under the OAuth 2.1 flow above)\n    openIdConnectUrl: https://dashboard.coresignal.com/.well-known/openid-configuration\n    jwks_uri: https://dashboard.coresignal.com/api/auth/jwks\n    userinfo_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/userinfo\n    end_session_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/end-session\n    id_token_signing_alg: [RS256]\n    subject_types: [public]\n    claims: [sub, iss, aud, exp, iat, sid, scope, azp, email, email_verified, name, picture, family_name, given_name]\n    prompt_values: [login, consent, create, select_account, none]\n    acr_values: ['urn:mace:incommon:iap:bronze']\n    sources: [well-known/coresignal-openid-configuration.json]\nlegacy_mcp:\n  endpoint: https://mcp.coresignal.com/mcp\n  scheme: apiKey\n  header: apikey\n  note: >-\n    The legacy MCP endpoint takes the same REST API key as a header (commonly passed through the\n    `mcp-remote` bridge). Its\
  \ tools/list is anonymously introspectable. Coresignal states it will\n    eventually be deprecated in favour of the OAuth-protected v2 endpoint.\nfailures:\n  - status: 401\n    meaning: No valid API Key was provided (REST), or no/invalid bearer token (MCP v2).\n    body_rest: '{\"detail\": \"...\"}'\n    body_mcp: '{\"error\": \"invalid_token\", \"error_description\": \"Authentication required\"}'\n    challenge_mcp: >-\n      WWW-Authenticate: Bearer error=\"invalid_token\",\n      resource_metadata=\"https://mcp.coresignal.com/.well-known/oauth-protected-resource/mcp/v2\"\ntransport:\n  https_required: true\n  note: >-\n    All requests must be made over HTTPS; HTTP requests fail or are redirected. See\n    security/coresignal-domain-security.yml for TLS/HSTS posture.\ngaps:\n  - No scopes or least-privilege model on either surface.\n  - No documented key expiry or forced rotation.\n  - No mTLS, no request signing, no IP allowlisting documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/authentication/coresignal-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Agentic Search
- B2B Data
- Companies
- Company Data
- Data as a Service
- Elasticsearch
- Employee Data
- Employees
- Enrichment
- Firmographics
- Job Postings
- Job
- Lead Generation
- People Data
- Sales Intelligence
- Talent Intelligence
- Web Data
---
