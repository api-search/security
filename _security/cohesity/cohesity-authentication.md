---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cohesity-cluster-v2-openapi.yml
  format: yaml
  label: Cohesity Helios REST API
  slug: helios-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohesity/refs/heads/main/openapi/cohesity-cluster-v2-openapi.yml
- filename: cohesity-cluster-v1-openapi.yml
  format: yaml
  label: Cohesity DataProtect REST API
  slug: dataprotect-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohesity/refs/heads/main/openapi/cohesity-cluster-v1-openapi.yml
- filename: cohesity-helios-reporting-openapi.yml
  format: yaml
  label: Cohesity Helios Reporting API
  slug: helios-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohesity/refs/heads/main/openapi/cohesity-helios-reporting-openapi.yml
- filename: cohesity-site-continuity-openapi.yml
  format: yaml
  label: Cohesity Site Continuity API
  slug: site-continuity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohesity/refs/heads/main/openapi/cohesity-site-continuity-openapi.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Cohesity Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cohesity secures its APIs with apiKey, oauth2, openIdConnect, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cohesity
provider_slug: cohesity
scheme_count: 4
schemes:
- description: The primary automation credential across every Cohesity surface. A Helios or cluster API key is created once in the UI (or from an authenticated session) and shown only once, then sent on every request in the `apiKey` header.
  in: header
  name: APIKeyHeader
  parameter: apiKey
  sources:
  - openapi/cohesity-cluster-v2-openapi.yml
  - openapi/cohesity-helios-reporting-openapi.yml
  - openapi/cohesity-site-continuity-openapi.yml
  type: apiKey
- authorizationUrl: https://helios.cohesity.com/oauth2/authorize
  description: Not declared in any published OpenAPI document; discovered from the live OIDC and RFC 8414 metadata Helios serves. Public clients are supported (token_endpoint_auth_method `none` with PKCE S256).
  flow: authorizationCode
  issuer: https://helios.cohesity.com
  jwksUri: https://helios.cohesity.com/oauth2/jwks.json
  name: Helios OAuth 2.0 / OIDC
  pkce:
  - S256
  revocationUrl: https://helios.cohesity.com/oauth2/revoke
  scopes_ref: scopes/cohesity-scopes.yml
  sources:
  - well-known/cohesity-openid-configuration.json
  tokenUrl: https://helios.cohesity.com/oauth2/token
  type: oauth2
- description: On-prem clusters accept username + password + domain at the access-token endpoint and return a token used on subsequent calls.
  name: Cluster access token
  scheme: bearer
  sources:
  - https://developers.cohesity.com/docs/getting-started
  type: http
- description: On-prem clusters also support a session-ID cookie obtained from an interactive login; this is the cookie used to mint an API key programmatically.
  in: cookie
  name: Cluster session ID
  sources:
  - https://developers.cohesity.com/docs/getting-started
  type: apiKey
slug: cohesity-authentication
source_filename: cohesity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  openapi/cohesity-cluster-v2-openapi.yml,\n  openapi/cohesity-helios-reporting-openapi.yml,\n  openapi/cohesity-site-continuity-openapi.yml (securityDefinitions), upgraded\n  with https://developers.cohesity.com/docs/getting-started and the live Helios\n  OAuth/OIDC discovery documents\ndocs: https://developers.cohesity.com/docs/getting-started\nsummary:\n  types: [apiKey, oauth2, openIdConnect, http]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: APIKeyHeader\n    type: apiKey\n    in: header\n    parameter: apiKey\n    sources:\n      - openapi/cohesity-cluster-v2-openapi.yml\n      - openapi/cohesity-helios-reporting-openapi.yml\n      - openapi/cohesity-site-continuity-openapi.yml\n    description: >-\n      The primary automation credential across every Cohesity surface. A Helios\n      or cluster API key is created once in the UI (or from an authenticated\n      session) and shown\
  \ only once, then sent on every request in the `apiKey`\n      header.\n  - name: Helios OAuth 2.0 / OIDC\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://helios.cohesity.com/oauth2/authorize\n    tokenUrl: https://helios.cohesity.com/oauth2/token\n    revocationUrl: https://helios.cohesity.com/oauth2/revoke\n    jwksUri: https://helios.cohesity.com/oauth2/jwks.json\n    issuer: https://helios.cohesity.com\n    pkce: [S256]\n    scopes_ref: scopes/cohesity-scopes.yml\n    sources: [well-known/cohesity-openid-configuration.json]\n    description: >-\n      Not declared in any published OpenAPI document; discovered from the live\n      OIDC and RFC 8414 metadata Helios serves. Public clients are supported\n      (token_endpoint_auth_method `none` with PKCE S256).\n  - name: Cluster access token\n    type: http\n    scheme: bearer\n    sources: [https://developers.cohesity.com/docs/getting-started]\n    description: >-\n      On-prem clusters accept username +\
  \ password + domain at the access-token\n      endpoint and return a token used on subsequent calls.\n  - name: Cluster session ID\n    type: apiKey\n    in: cookie\n    sources: [https://developers.cohesity.com/docs/getting-started]\n    description: >-\n      On-prem clusters also support a session-ID cookie obtained from an\n      interactive login; this is the cookie used to mint an API key programmatically.\nsurfaces:\n  - surface: Helios (SaaS control plane)\n    methods: [api-key, username-password-ui, oauth2]\n    mfa: >-\n      Multi-factor authentication is supported for interactive sign-in. Cohesity\n      documents that enabling MFA does NOT support automation - an important\n      operational constraint for any agent or CI credential.\n    docs: https://developers.cohesity.com/docs/getting-started\n  - surface: On-prem cluster (DataProtect)\n    methods: [access-token, session-id, api-key]\n    mfa: Supported on all three methods when enabled on the cluster.\n    docs: https://developers.cohesity.com/docs/getting-started\n\
  \  - surface: Gaia Data Insights / Gaia MCP\n    methods: [api-key]\n    header: apiKey\n    privilege: GAIA_VIEW\n    docs: https://learn.microsoft.com/en-us/connectors/cohesitygaiamcp/\ncredential_lifecycle:\n  rotation_docs: https://docs.cohesity.com/WebHelios/Content/Helios/Access%20Management.htm\n  note: >-\n    API keys are displayed exactly once at creation and cannot be retrieved\n    afterwards; rotation means issuing a new key and revoking the old one from\n    Helios Access Management. OAuth tokens are revocable at the documented\n    revocation endpoint.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cohesity/refs/heads/main/authentication/cohesity-authentication.yml
summary_line: apiKey/oauth2/openIdConnect/http · 4 schemes
tags:
- Automation
- Backup
- Cyber Resilience
- Data Management
- Data Protection
- Data Security
- DataProtect
- Disaster Recovery
- Helios
- Orchestration
- Ransomware Recovery
- Site Continuity
- Reporting
- Model Context Protocol
- Enterprise Storage
---
