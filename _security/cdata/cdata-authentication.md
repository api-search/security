---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cdata-rest-api-openapi.yml
  format: yaml
  label: CData SQL API
  slug: sql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-openapi.yml
- filename: cdata-rest-api-openapi.yml
  format: yaml
  label: CData Metadata API
  slug: metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-openapi.yml
- filename: cdata-rest-api-openapi.yml
  format: yaml
  label: CData Log API
  slug: log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-openapi.yml
- filename: cdata-rest-api-embedded-openapi.yml
  format: yaml
  label: CData Connection API
  slug: connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-embedded-openapi.yml
- filename: cdata-rest-api-embedded-openapi.yml
  format: yaml
  label: CData Job API
  slug: job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-embedded-openapi.yml
- filename: cdata-rest-api-embedded-openapi.yml
  format: yaml
  label: CData Account API
  slug: account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-embedded-openapi.yml
- filename: cdata-rest-api-openapi.yml
  format: yaml
  label: CData Audit API
  slug: audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-rest-api-openapi.yml
- filename: cdata-odata-api-openapi.yml
  format: yaml
  label: CData OData API
  slug: odata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-odata-api-openapi.yml
- filename: cdata-mcp-api-openapi.yml
  format: yaml
  label: CData Connect AI MCP Server
  slug: mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-mcp-api-openapi.yml
- filename: cdata-management-api-openapi.yml
  format: yaml
  label: CData Connect AI Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-management-api-openapi.yml
- filename: cdata-mcp-api-embedded-openapi.yml
  format: yaml
  label: CData Connect AI Embed MCP Server
  slug: mcp-embedded
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-mcp-api-embedded-openapi.yml
- filename: cdata-openapi-api-openapi.yml
  format: yaml
  label: CData Connect AI OpenAPI API
  slug: openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-openapi-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cdata Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CData secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CData
provider_slug: cdata
scheme_count: 3
schemes:
- flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://cloud-login.cdata.com/oauth/token
  name: oauth2
  sources:
  - openapi/cdata-management-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  description: JWT token authentication. Include the token in the Authorization header as 'Bearer <token>'.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cdata-mcp-api-embedded-openapi.yml
  - openapi/cdata-rest-api-embedded-openapi.yml
  type: http
- description: Basic Authentication with username and password. Use your PAT as the password. You can get your PAT from Connect AI by selecting **Settings** > **Access Tokens**.
  name: Basic
  scheme: basic
  sources:
  - openapi/cdata-mcp-api-openapi.yml
  - openapi/cdata-odata-api-openapi.yml
  - openapi/cdata-openapi-api-openapi.yml
  - openapi/cdata-rest-api-openapi.yml
  type: http
slug: cdata-authentication
source_filename: cdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\ndocs:\n- https://docs.cloud.cdata.com/en/API/Authentication.md\n- https://docs.cloud.cdata.com/en/API/Authentication-Embedded.md\n- https://docs.cloud.cdata.com/en/API/MCP.md\n- https://docs.cloud.cdata.com/en/Settings/Personal-Access-Tokens\nsource: openapi/cdata-management-api-openapi.yml, openapi/cdata-mcp-api-embedded-openapi.yml,\n  openapi/cdata-mcp-api-openapi.yml, openapi/cdata-odata-api-openapi.yml, openapi/cdata-openapi-api-openapi.yml,\n  openapi/cdata-rest-api-embedded-openapi.yml, openapi/cdata-rest-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://cloud-login.cdata.com/oauth/token\n    scopes: 4\n  sources:\n  - openapi/cdata-management-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token authentication. Include\
  \ the token in the Authorization header as 'Bearer\n    <token>'.\n  sources:\n  - openapi/cdata-mcp-api-embedded-openapi.yml\n  - openapi/cdata-rest-api-embedded-openapi.yml\n- name: Basic\n  type: http\n  scheme: basic\n  description: Basic Authentication with username and password. Use your PAT as the password.\n    You can get your PAT from Connect AI by selecting **Settings** > **Access Tokens**.\n  sources:\n  - openapi/cdata-mcp-api-openapi.yml\n  - openapi/cdata-odata-api-openapi.yml\n  - openapi/cdata-openapi-api-openapi.yml\n  - openapi/cdata-rest-api-openapi.yml\n\n# --- SEARCHED enrichment, 2026-09-05 -------------------------------------------------\n# Derived from the seven first-party specs above, then upgraded against CData's own\n# published authentication pages and the live discovery documents in well-known/.\ndocs_detail:\n  connect_ai:\n    url: https://docs.cloud.cdata.com/en/API/Authentication.md\n    methods:\n    - name: HTTP Basic\n      username: the registered\
  \ user's email address (e.g. user@cdata.com)\n      password: >-\n        a Personal Access Token (PAT) generated on the Settings > Personal Access Tokens\n        page — never the account password.\n      encoding: Base64 of \"email:PAT\" in the Authorization header\n      applies_to: [REST API, OData API, OpenAPI API, MCP data server]\n    - name: OAuth 2.0 client credentials\n      issuer: https://cloud-login.cdata.com/\n      token_endpoint: https://cloud-login.cdata.com/oauth/token\n      authorization_endpoint: https://cloud-login.cdata.com/authorize\n      credentials: >-\n        Client Id and Client Secret from a service account, created on the Service Accounts\n        tab of the Users page.\n      intended_for: scripts, jobs and external services with no human user\n      applies_to: [Management API, REST API]\n      discovery: well-known/cdata-cloud-login-openid-configuration.json\n  connect_ai_embed:\n    url: https://docs.cloud.cdata.com/en/API/Authentication-Embedded.md\n\
  \    methods:\n    - name: JWT bearer\n      note: >-\n        All requests to the Connect AI Embed API authenticate with a JSON Web Token minted\n        by the ISV. Matches the BearerAuth scheme in the Embed specs above.\n  mcp:\n    url: https://docs.cloud.cdata.com/en/API/MCP.md\n    methods:\n    - name: OAuth 2.1 (authorization code + PKCE)\n      authorization_server: https://mcp.cloud.cdata.com\n      authorization_endpoint: https://mcp.cloud.cdata.com/authorize\n      token_endpoint: https://mcp.cloud.cdata.com/token\n      registration_endpoint: https://mcp.cloud.cdata.com/register\n      code_challenge_methods: [S256]\n      token_endpoint_auth_methods: [none]\n      scopes: [openid, profile, email, offline_access]\n      discovery: well-known/cdata-mcp-oauth-authorization-server.json\n      protected_resource_metadata: well-known/cdata-mcp-oauth-protected-resource.json\n      note: >-\n        A live anonymous POST to https://mcp.cloud.cdata.com/mcp returns HTTP 401 with a\n\
  \        correct RFC 9728 WWW-Authenticate challenge naming the resource_metadata document.\n        This is the strongest auth signal in the record: it was observed, not read.\n    - name: HTTP Basic\n      note: Connect AI user id plus PAT, for MCP clients that do not implement OAuth.\nenterprise_identity:\n  sso:\n    url: https://docs.cloud.cdata.com/en/SCIM/SSO.md\n    note: Enterprise SSO with multiple identity providers; listed as a Business-tier feature.\n  scim:\n    url: https://docs.cloud.cdata.com/en/SCIM.md\n    version: '2.0'\n    note: >-\n      SCIM 2.0 user and group provisioning from Okta, Entra ID and Ping Identity, plus\n      Just-in-Time provisioning on first SSO login. The Management API exposes\n      `scim_managed` on user records and refuses name updates on SCIM-managed users,\n      because the IdP owns those fields. See conformance/cdata-conformance.yml.\n  passthrough_identity:\n    note: >-\n      Business tier passes each end user's own credentials through\
  \ to the source system at\n      query time, so an agent inherits that user's permissions rather than sharing a\n      service credential. Published on https://www.cdata.com/ai/pricing/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/authentication/cdata-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Data
- Data Access
- Data Connectivity
- Databases
- NoSQL
- SQL
---
