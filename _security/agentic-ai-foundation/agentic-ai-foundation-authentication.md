---
api_key_in: []
api_specs:
- filename: agentic-ai-foundation-mcp-registry-openapi.yaml
  format: yaml
  label: Official MCP Registry API
  slug: mcp-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentic-ai-foundation/refs/heads/main/openapi/agentic-ai-foundation-mcp-registry-openapi.yaml
auth_types: []
description: 'Authentication profile across the AAIF-hosted surfaces that are actually callable. The Official MCP Registry API is read-anonymous / write-bearer: every GET and the validate endpoint are unauthenticated, and the four write operations require a Registry JWT minted by one of five token-exchange endpoints. The MCP endpoint on modelcontextprotocol.io is fully anonymous.'
kind: authentication
layout: security
method: derived
name: Agentic Ai Foundation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agentic AI Foundation declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Agentic AI Foundation
provider_slug: agentic-ai-foundation
scheme_count: 0
schemes: []
slug: agentic-ai-foundation-authentication
source_filename: agentic-ai-foundation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: derived\nsource: openapi/agentic-ai-foundation-mcp-registry-openapi.yaml + live probes of registry.modelcontextprotocol.io and modelcontextprotocol.io/mcp\nprovider: Agentic AI Foundation\nproviderId: agentic-ai-foundation\ndescription: >-\n  Authentication profile across the AAIF-hosted surfaces that are actually callable. The Official MCP\n  Registry API is read-anonymous / write-bearer: every GET and the validate endpoint are unauthenticated,\n  and the four write operations require a Registry JWT minted by one of five token-exchange endpoints.\n  The MCP endpoint on modelcontextprotocol.io is fully anonymous.\napis:\n  - name: Official MCP Registry\n    baseURL: https://registry.modelcontextprotocol.io\n    spec: openapi/agentic-ai-foundation-mcp-registry-openapi.yaml\n    schemes:\n      - id: bearer\n        type: http\n        scheme: bearer\n        bearerFormat: JWT\n        in: header\n        header: Authorization\n        applied_to:\n\
  \          - publish-server-v0.1\n          - edit-server-v0.1\n          - update-server-status-v0.1\n          - update-server-all-versions-status-v0.1\n          - publish-server-v0\n          - edit-server-v0\n          - update-server-status-v0\n          - update-server-all-versions-status-v0\n        defect: >-\n          The scheme name `bearer` is referenced by these eight operations but components.securitySchemes\n          is ABSENT from the published document, so the reference dangles and a code generator produces a\n          client with no auth. Recorded, not corrected in place — the correction is in\n          overlays/agentic-ai-foundation-mcp-registry-overlay.yaml.\n    token_exchange:\n      description: >-\n        Five ways to obtain the Registry JWT. Each is a POST that trades an externally-issued credential\n        for a registry-scoped token; there is no username/password and no long-lived API key.\n      endpoints:\n        - path: /v0.1/auth/github-at\n      \
  \    operationId: exchange-github-token-v0.1\n          credential: GitHub OAuth access token\n        - path: /v0.1/auth/github-oidc\n          operationId: exchange-github-oidc-token-v0.1\n          credential: GitHub Actions OIDC token\n        - path: /v0.1/auth/oidc\n          operationId: exchange-oidc-token-v0.1\n          credential: Generic OIDC ID token\n        - path: /v0.1/auth/dns\n          operationId: exchange-dns-token-v0.1\n          credential: DNS TXT record signature proving domain control\n        - path: /v0.1/auth/http\n          operationId: exchange-http-token-v0.1\n          credential: HTTP signature proving control of a well-known path on the namespace domain\n      note: >-\n        The same five endpoints exist under the /v0 prefix. GET /v0/health returns a github_client_id\n        field, confirming a GitHub OAuth app backs the github-at flow.\n    anonymous_operations:\n      - list-servers-v0.1\n      - get-server-versions-v0.1\n      - get-server-version-v0.1\n\
  \      - validate-server-v0.1\n      - get-health-v0.1\n      - ping-v0.1\n      - get-version-v0.1\n    identity_model: >-\n      Namespace ownership. A publisher proves control of the namespace it is publishing under — a GitHub\n      org/user for io.github.* names, or DNS/HTTP proof of a domain for reverse-DNS names — and the\n      registry issues a JWT scoped to that namespace.\n  - name: MCP documentation server\n    baseURL: https://modelcontextprotocol.io/mcp\n    schemes:\n      - id: none\n        type: none\n        description: >-\n          Probed anonymously 2026-08-30: tools/list returned HTTP 200 with the full tool set. No OAuth\n          challenge, no WWW-Authenticate header, no API key. /.well-known/oauth-authorization-server and\n          /.well-known/oauth-protected-resource both 404 on this host.\n    anonymous: true\noauth2: false\nopenid_connect:\n  consumed: true\n  provided: false\n  note: >-\n    The registry CONSUMES OIDC ID tokens (including GitHub Actions\
  \ OIDC) to mint its own JWT, but it does\n    not act as an OpenID Provider. No /.well-known/openid-configuration is served on any host; the\n    versioned paths /v0/.well-known/openid-configuration and /v0.1/.well-known/openid-configuration were\n    probed and 404.\ndocs:\n  - https://github.com/modelcontextprotocol/registry/tree/main/docs\n  - https://registry.modelcontextprotocol.io/docs\nmaintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentic-ai-foundation/refs/heads/main/authentication/agentic-ai-foundation-authentication.yml
summary_line: 0 schemes
tags:
- AI Agents
- Linux Foundation
- Open-Source
- Standards
- MCP
- Agentic AI
- Interoperability
- Agent Protocols
- A2A
- AGENTS.md
- Open Governance
---
