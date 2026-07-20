---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: First Resonance Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: First Resonance secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: First Resonance
provider_slug: first-resonance
scheme_count: 1
schemes:
- authorization_header: 'Authorization: <access_token>'
  environments:
  - api: https://api.buildwithion.com
    auth_server: auth.buildwithion.com
    env: production
    realm_token_endpoint: https://auth-production-pub.buildwithion.com/realms/api-keys/protocol/openid-connect/token
  - api: https://staging-api.buildwithion.com
    auth_server: staging-auth.buildwithion.com
    env: staging-sandbox
  - api: https://api-staging-gov.buildwithion.com
    auth_server: auth-staging-gov.buildwithion.com
    env: gov-staging
  - api: https://api-production-gov.buildwithion.com
    auth_server: auth-production-gov.buildwithion.com
    env: gov-production
  - api: https://api-staging-aus.buildwithion.com
    auth_server: auth-staging-aus.buildwithion.com
    env: aus-staging
  - api: https://api-production-aus.buildwithion.com
    auth_server: auth-production-aus.buildwithion.com
    env: aus-production
  flow: clientCredentials
  grant_type: client_credentials
  name: apiKeyClientCredentials
  token_request: "curl -X POST \\\n  --data-urlencode \"grant_type=client_credentials\" \\\n  -d \"client_id=CLIENT_ID\" \\\n  -d \"client_secret=CLIENT_SECRET\" \\\n  https://<AUTH_SERVER>/realms/api-keys/protocol/openid-connect/token\n"
  type: oauth2
slug: first-resonance-authentication
source_filename: first-resonance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://manual.firstresonance.io/api/access-tokens\ndocs:\n- https://manual.firstresonance.io/api/access-tokens\n- https://manual.firstresonance.io/api/api-keys\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  model: >-\n    OAuth 2.0 client-credentials. An ION API key is a clientId/clientSecret pair\n    created per Organization (via UI or API). It is exchanged for a JWT access\n    token at a Keycloak \"api-keys\" realm token endpoint, then sent on the GraphQL\n    request in the Authorization header.\n  identity_provider: Keycloak (realm \"api-keys\")\n  permission_model: >-\n    An API key inherits (freezes) the permissions its creating user held at the\n    moment of generation (RBAC via the APIKeyObject permission family). Service\n    accounts are recommended over personal keys to decouple keys from user\n    deactivation and preserve an audit trail. This is a permission model rather\n    than an\
  \ OAuth scope model, so no granular API scope reference is published.\nschemes:\n- name: apiKeyClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  grant_type: client_credentials\n  token_request: |\n    curl -X POST \\\n      --data-urlencode \"grant_type=client_credentials\" \\\n      -d \"client_id=CLIENT_ID\" \\\n      -d \"client_secret=CLIENT_SECRET\" \\\n      https://<AUTH_SERVER>/realms/api-keys/protocol/openid-connect/token\n  authorization_header: 'Authorization: <access_token>'\n  environments:\n  - {env: production, auth_server: auth.buildwithion.com, api: https://api.buildwithion.com, realm_token_endpoint: https://auth-production-pub.buildwithion.com/realms/api-keys/protocol/openid-connect/token}\n  - {env: staging-sandbox, auth_server: staging-auth.buildwithion.com, api: https://staging-api.buildwithion.com}\n  - {env: gov-staging, auth_server: auth-staging-gov.buildwithion.com, api: https://api-staging-gov.buildwithion.com}\n  - {env: gov-production, auth_server:\
  \ auth-production-gov.buildwithion.com, api: https://api-production-gov.buildwithion.com}\n  - {env: aus-staging, auth_server: auth-staging-aus.buildwithion.com, api: https://api-staging-aus.buildwithion.com}\n  - {env: aus-production, auth_server: auth-production-aus.buildwithion.com, api: https://api-production-aus.buildwithion.com}\nnotes:\n- Keys are environment-specific (a production key does not work in sandbox).\n- Generating a new key pair does not invalidate existing keys; keys must be disabled manually.\n- Keys are auto-disabled when the creating user is deactivated (hence the service-account recommendation).\n- SSO (Okta SAML) and enforced MFA are available for interactive user login, separate from API-key auth.\n- The beta MCP server authenticates separately via OAuth 2.1 DCR (see mcp/first-resonance-mcp.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-resonance/refs/heads/main/authentication/first-resonance-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Infrastructure
- Manufacturing
- MES
- Factory Operating System
- Hardware
- Aerospace
- GraphQL
- Traceability
- Supply Chain
---
