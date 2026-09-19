---
anonymous_access: false
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Boltmcp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: BoltMCP secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: BoltMCP
provider_slug: boltmcp
scheme_count: 1
schemes:
- discovery: Services fetch the OIDC discovery document from the PUBLIC issuer URL server-side, which is why the troubleshooting docs call out split-horizon DNS as a failure mode.
  issuer_template: https://auth.{global.domain}/realms/boltmcp
  name: oidc
  provider: keycloak
  realm: boltmcp
  sources:
  - https://install.boltmcp.io/docs/troubleshooting
  type: openIdConnect
slug: boltmcp-authentication
source_filename: boltmcp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://install.boltmcp.io/docs/sign-in\ndocs: https://install.boltmcp.io/docs/sign-in\nnote: >-\n  Derived from no OpenAPI - BoltMCP publishes none. This profile is read from the published\n  installation documentation, which describes the identity layer of a BoltMCP deployment in detail.\n  Every surface in a BoltMCP install authenticates through OpenID Connect against an identity\n  provider the customer runs; the chart bundles Keycloak 26.7.0 as the default, and the architecture\n  page names Okta, Microsoft Entra and Ping Identity as supported alternatives.\nsummary:\n  types: [openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials]\n  identity_provider_default: keycloak\n  identity_provider_byo: [Okta, Microsoft Entra, Ping Identity]\n  mfa: delegated to the identity provider\nschemes:\n- name: oidc\n  type: openIdConnect\n  provider: keycloak\n  realm: boltmcp\n  issuer_template:\
  \ https://auth.{global.domain}/realms/boltmcp\n  discovery: >-\n    Services fetch the OIDC discovery document from the PUBLIC issuer URL server-side, which is why\n    the troubleshooting docs call out split-horizon DNS as a failure mode.\n  sources: [https://install.boltmcp.io/docs/troubleshooting]\nclients:\n- client_id: boltmcp-web\n  purpose: the dashboard authenticating end users\n  secret_key: web-client-secret\n- client_id: boltmcp-mcp-server\n  purpose: the MCP servers authenticating users and agents\n  secret_key: mcp-server-client-secret\n- client_id: boltmcp-rest-api\n  purpose: the internal REST API verifying tokens\n  status: redundant as of chart 0.5.x - the migration guide says it may be deleted\n- client_id: boltmcp-rest-api-to-keycloak\n  purpose: the REST API's Keycloak Admin service account\n  secret_key: rest-api-to-keycloak-client-secret\n- client_id: boltmcp-mcp-server-to-rest-api\n  purpose: pre-configured so a first MCP server can authenticate users with the internal\
  \ API\n- client_id: boltmcp-mcp-server-to-keycloak\n  purpose: pre-configured so a first MCP server can authenticate users with the Keycloak Admin API\ndynamic_client_registration:\n  supported: true\n  mechanism: CIMD client policies in the boltmcp Keycloak realm\n  note: >-\n    \"MCP clients such as Claude don't need a pre-configured client: they register themselves via the\n    realm's CIMD client policies when connecting.\" Quoted verbatim from the Sign In documentation.\n  source: https://install.boltmcp.io/docs/sign-in\nuser_requirements:\n  required_claims: [email, given_name]\n  note: >-\n    BoltMCP requires users to have an email and a first name to sign in; the auto-provisioned\n    boltmcp_admin user gets both at realm-import time.\n  source: https://install.boltmcp.io/docs/troubleshooting\nsecrets_management:\n  store: HashiCorp Vault (bundled) via Kubernetes auth\n  kv_path_prefix: boltmcp/server-env-api-cred\n  rotation_procedure: https://install.boltmcp.io/docs/rotating-secrets\n\
  \  external_options: [External Secrets Operator, Sealed Secrets, SOPS]\ngaps:\n- No public, vendor-operated authentication surface exists - every credential is provisioned inside\n  the customer's own deployment.\n- No OpenAPI securitySchemes could be read, because no OpenAPI is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boltmcp/refs/heads/main/authentication/boltmcp-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- MCP
- Agents
- Artificial Intelligence
- Kubernetes
- Self-Hosted
- Enterprise
- Identity
- Developer Tools
---
