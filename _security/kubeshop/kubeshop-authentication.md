---
api_key_in: []
api_specs:
- filename: kubeshop-testkube-control-plane-openapi-original.yml
  format: yaml
  label: Testkube Control Plane API
  slug: testkube-control-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubeshop/refs/heads/main/openapi/kubeshop-testkube-control-plane-openapi-original.yml
- filename: kubeshop-testkube-agent-openapi-original.yml
  format: yaml
  label: Testkube Standalone Agent API
  slug: testkube-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubeshop/refs/heads/main/openapi/kubeshop-testkube-agent-openapi-original.yml
- filename: kubeshop-testkube-openapi-original.yml
  format: yaml
  label: Testkube API (open source)
  slug: testkube-oss
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubeshop/refs/heads/main/openapi/kubeshop-testkube-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Kubeshop Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kubeshop secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kubeshop
provider_slug: kubeshop
scheme_count: 2
schemes:
- applies_to: REST API (control plane and agent)
  header: 'Authorization: Bearer <API_TOKEN>'
  name: BearerAuth
  note: Only the control-plane spec declares this scheme. The standalone-agent and open-source specs declare no securitySchemes at all, though the deployed API is bearer-authenticated the same way.
  scheme: bearer
  sources:
  - openapi/kubeshop-testkube-control-plane-openapi-original.yml
  token_issuance: Organization Settings → API Tokens in the Testkube dashboard
  type: http
- applies_to: https://api.testkube.io/mcp
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://api.testkube.io/mcp/auth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.testkube.io/mcp/auth/register
    revocationUrl: https://api.testkube.io/mcp/auth/revoke
    scopes:
      mcp:full: Full access to the Testkube MCP endpoint for the authorized organization and environment
    tokenUrl: https://api.testkube.io/mcp/auth/token
  name: TestkubeMCPOAuth
  note: Discovered live. An unauthenticated request to /mcp returns a WWW-Authenticate Bearer challenge carrying resource_metadata and scope="mcp:full". Shipped in v2.10.0 and hardened in v2.11.1.
  sources:
  - https://api.testkube.io/.well-known/oauth-authorization-server
  - https://api.testkube.io/.well-known/oauth-protected-resource
  standards:
  - RFC 8414
  - RFC 9728
  - RFC 7591
  - OAuth 2.1
  type: oauth2
slug: kubeshop-authentication
source_filename: kubeshop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kubeshop-testkube-control-plane-openapi-original.yml\ndocs: https://docs.testkube.io/articles/mcp-security\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  oauth2_scope: mcp:full\n  note: >-\n    The REST surface is bearer-token authenticated with a long-lived API token. OAuth 2.1\n    applies to the MCP endpoint only; it is not an alternative for the REST API.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer <API_TOKEN>'\n  applies_to: REST API (control plane and agent)\n  token_issuance: Organization Settings → API Tokens in the Testkube dashboard\n  sources:\n  - openapi/kubeshop-testkube-control-plane-openapi-original.yml\n  note: >-\n    Only the control-plane spec declares this scheme. The standalone-agent and\n    open-source specs declare no securitySchemes at all, though the deployed API is\n    bearer-authenticated\
  \ the same way.\n- name: TestkubeMCPOAuth\n  type: oauth2\n  applies_to: https://api.testkube.io/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.testkube.io/mcp/auth/authorize\n    tokenUrl: https://api.testkube.io/mcp/auth/token\n    revocationUrl: https://api.testkube.io/mcp/auth/revoke\n    registrationUrl: https://api.testkube.io/mcp/auth/register\n    pkce: S256\n    scopes:\n      mcp:full: Full access to the Testkube MCP endpoint for the authorized organization and environment\n  dynamic_client_registration: true\n  standards: [RFC 8414, RFC 9728, RFC 7591, OAuth 2.1]\n  sources:\n  - https://api.testkube.io/.well-known/oauth-authorization-server\n  - https://api.testkube.io/.well-known/oauth-protected-resource\n  note: >-\n    Discovered live. An unauthenticated request to /mcp returns a WWW-Authenticate Bearer\n    challenge carrying resource_metadata and scope=\"mcp:full\". Shipped in v2.10.0 and\n    hardened in v2.11.1.\nauthorization:\n  model:\
  \ rbac\n  boundaries: [organization, environment, resource group, team]\n  note: >-\n    Permissions are scoped through organization membership roles, teams and resource\n    groups. HTTP 403 signals a permission or feature-disabled condition; HTTP 402 signals a\n    missing Pro subscription rather than an authorization failure.\n  audit_logs: >-\n    The control plane exposes application audit logs (listApplicationAuditLogs,\n    exportApplicationAuditLog); audit logs are listed as a paid entitlement on the pricing page.\ncross_ref:\n  scopes: scopes/kubeshop-scopes.yml\n  conventions: conventions/kubeshop-conventions.yml\n  mcp: mcp/kubeshop-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubeshop/refs/heads/main/authentication/kubeshop-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Testing
- Kubernetes
- Continuous Integration
- Developer Tools
- Test Automation
- Observability
- DevOps
- Cloud Native
- Quality Assurance
- Open Source
- Model Context Protocol
---
