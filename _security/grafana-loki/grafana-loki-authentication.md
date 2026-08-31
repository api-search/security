---
api_key_in: []
auth_types: []
description: 'Grafana Loki deliberately ships no authentication. The Loki HTTP API reference states plainly: "authorization is not part of the Loki API. Authorization needs to be done separately, for example, using an open-source load-balancer such as NGINX." What Loki does carry natively is tenancy — the X-Scope-OrgID header — which is an isolation boundary, not a credential. Authentication is supplied by whatever fronts Loki: a reverse proxy for self-hosted deployments, HTTP Basic with an access policy token for Grafana Cloud Logs and Grafana Enterprise Logs, and OAuth 2.1 for the hosted Grafana Cloud MCP server.'
kind: authentication
layout: security
method: searched
name: Grafana Loki Authentication
name_suffix: Authentication
oauth_flows: []
overview: Grafana Loki declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Grafana Loki
provider_slug: grafana-loki
scheme_count: 6
schemes:
- description: 'Identifies the tenant whose data is being written or read when Loki runs with auth_enabled: true. Multiple tenants may be queried at once by pipe-separating them (X-Scope-OrgID: Tenant1|Tenant2|Tenant3). This header is an identifier, not a secret — Loki trusts it, which is why an authenticating proxy must sit in front and set it.'
  docs: https://grafana.com/docs/loki/latest/operations/multi-tenancy/
  id: tenant-header
  in: header
  is_credential: false
  name: X-Scope-OrgID
  surface: Loki HTTP API (self-hosted, multi-tenant mode)
  type: apiKey
- description: HTTP Basic authentication where the username is the tenant name (pipe-separated for multiple tenants) and the password is an access policy token. Access policies carry scopes such as logs:write, logs:read and logs:delete; the deletion endpoints require a token whose access policy holds logs:delete for the named tenant.
  docs: https://grafana.com/docs/loki/latest/reference/loki-http-api/
  id: basic-access-policy-token
  scheme: basic
  scopes_referenced:
  - logs:read
  - logs:write
  - logs:delete
  surface: Grafana Cloud Logs / Grafana Enterprise Logs
  type: http
- description: logcli sends an Authorization header when LOKI_BEARER_TOKEN or LOKI_BEARER_TOKEN_FILE is set, which is the supported path when Loki sits behind a proxy that validates bearer tokens.
  docs: https://grafana.com/docs/loki/latest/query/logcli/getting-started/
  id: bearer-token
  scheme: bearer
  surface: Loki behind an authenticating proxy
  type: http
- description: logcli accepts --cert / --key (LOKI_CLIENT_CERT_PATH, LOKI_CLIENT_KEY_PATH) and --ca-cert (LOKI_CA_CERT_PATH), so client-certificate authentication against a TLS-terminating proxy is a first-class supported path.
  docs: https://grafana.com/docs/loki/latest/query/logcli/getting-started/
  id: mtls
  surface: Loki HTTP API (client certificates)
  type: mutualTLS
- authorization_endpoint: https://mcp.grafana.com/mcp/oauth/authorize
  description: OAuth 2.1 authorization code with PKCE (S256) and dynamic client registration. Scopes grafana:read, grafana:query and grafana:write. Metadata published anonymously at /.well-known/oauth-authorization-server (RFC 8414) and /.well-known/oauth-protected-resource (RFC 9728).
  docs: https://grafana.com/docs/grafana-cloud/ai-tools/mcp-servers/cloud-mcp/
  id: mcp-oauth
  registration_endpoint: https://mcp.grafana.com/mcp/oauth/register
  scopes:
  - grafana:read
  - grafana:query
  - grafana:write
  surface: Grafana Cloud MCP server (https://mcp.grafana.com/mcp)
  token_endpoint: https://mcp.grafana.com/mcp/oauth/token
  type: oauth2
- description: The open-source Grafana MCP server authenticates to Grafana with a service account token supplied as GRAFANA_SERVICE_ACCOUNT_TOKEN alongside GRAFANA_URL. An optional caller-auth token (MCP_GRAFANA_SERVER_TOKEN) gates clients of the MCP listener itself.
  docs: https://github.com/grafana/mcp-grafana
  id: service-account-token
  in: header
  name: Authorization
  surface: grafana/mcp-grafana (open source MCP server)
  type: apiKey
slug: grafana-loki-authentication
source_filename: grafana-loki-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://grafana.com/docs/loki/latest/reference/loki-http-api/\nname: Grafana Loki authentication\ndescription: >-\n  Grafana Loki deliberately ships no authentication. The Loki HTTP API reference states plainly:\n  \"authorization is not part of the Loki API. Authorization needs to be done separately, for example,\n  using an open-source load-balancer such as NGINX.\" What Loki does carry natively is tenancy — the\n  X-Scope-OrgID header — which is an isolation boundary, not a credential. Authentication is supplied\n  by whatever fronts Loki: a reverse proxy for self-hosted deployments, HTTP Basic with an access\n  policy token for Grafana Cloud Logs and Grafana Enterprise Logs, and OAuth 2.1 for the hosted\n  Grafana Cloud MCP server.\nnative_auth: false\nnative_auth_statement: >-\n  \"Note that authorization is not part of the Loki API. Authorization needs to be done separately,\n  for example, using an open-source load-balancer\
  \ such as NGINX.\" —\n  https://grafana.com/docs/loki/latest/reference/loki-http-api/\nschemes:\n  - id: tenant-header\n    type: apiKey\n    in: header\n    name: X-Scope-OrgID\n    is_credential: false\n    surface: Loki HTTP API (self-hosted, multi-tenant mode)\n    description: >-\n      Identifies the tenant whose data is being written or read when Loki runs with auth_enabled:\n      true. Multiple tenants may be queried at once by pipe-separating them\n      (X-Scope-OrgID: Tenant1|Tenant2|Tenant3). This header is an identifier, not a secret — Loki\n      trusts it, which is why an authenticating proxy must sit in front and set it.\n    docs: https://grafana.com/docs/loki/latest/operations/multi-tenancy/\n  - id: basic-access-policy-token\n    type: http\n    scheme: basic\n    surface: Grafana Cloud Logs / Grafana Enterprise Logs\n    description: >-\n      HTTP Basic authentication where the username is the tenant name (pipe-separated for multiple\n      tenants) and the password\
  \ is an access policy token. Access policies carry scopes such as\n      logs:write, logs:read and logs:delete; the deletion endpoints require a token whose access\n      policy holds logs:delete for the named tenant.\n    scopes_referenced: [logs:read, logs:write, logs:delete]\n    docs: https://grafana.com/docs/loki/latest/reference/loki-http-api/\n  - id: bearer-token\n    type: http\n    scheme: bearer\n    surface: Loki behind an authenticating proxy\n    description: >-\n      logcli sends an Authorization header when LOKI_BEARER_TOKEN or LOKI_BEARER_TOKEN_FILE is set,\n      which is the supported path when Loki sits behind a proxy that validates bearer tokens.\n    docs: https://grafana.com/docs/loki/latest/query/logcli/getting-started/\n  - id: mtls\n    type: mutualTLS\n    surface: Loki HTTP API (client certificates)\n    description: >-\n      logcli accepts --cert / --key (LOKI_CLIENT_CERT_PATH, LOKI_CLIENT_KEY_PATH) and --ca-cert\n      (LOKI_CA_CERT_PATH), so client-certificate\
  \ authentication against a TLS-terminating proxy is a\n      first-class supported path.\n    docs: https://grafana.com/docs/loki/latest/query/logcli/getting-started/\n  - id: mcp-oauth\n    type: oauth2\n    surface: Grafana Cloud MCP server (https://mcp.grafana.com/mcp)\n    description: >-\n      OAuth 2.1 authorization code with PKCE (S256) and dynamic client registration. Scopes\n      grafana:read, grafana:query and grafana:write. Metadata published anonymously at\n      /.well-known/oauth-authorization-server (RFC 8414) and /.well-known/oauth-protected-resource\n      (RFC 9728).\n    authorization_endpoint: https://mcp.grafana.com/mcp/oauth/authorize\n    token_endpoint: https://mcp.grafana.com/mcp/oauth/token\n    registration_endpoint: https://mcp.grafana.com/mcp/oauth/register\n    scopes: [grafana:read, grafana:query, grafana:write]\n    docs: https://grafana.com/docs/grafana-cloud/ai-tools/mcp-servers/cloud-mcp/\n  - id: service-account-token\n    type: apiKey\n    in: header\n\
  \    name: Authorization\n    surface: grafana/mcp-grafana (open source MCP server)\n    description: >-\n      The open-source Grafana MCP server authenticates to Grafana with a service account token\n      supplied as GRAFANA_SERVICE_ACCOUNT_TOKEN alongside GRAFANA_URL. An optional caller-auth token\n      (MCP_GRAFANA_SERVER_TOKEN) gates clients of the MCP listener itself.\n    docs: https://github.com/grafana/mcp-grafana\nscheme_count: 6\nenvironment_variables:\n  - {name: LOKI_ADDR, purpose: Loki base address for logcli}\n  - {name: LOKI_USERNAME, purpose: HTTP Basic username}\n  - {name: LOKI_PASSWORD, purpose: HTTP Basic password / access policy token}\n  - {name: LOKI_ORG_ID, purpose: sets X-Scope-OrgID}\n  - {name: LOKI_BEARER_TOKEN, purpose: Authorization bearer token}\n  - {name: LOKI_BEARER_TOKEN_FILE, purpose: file containing the bearer token}\n  - {name: LOKI_CLIENT_CERT_PATH, purpose: client certificate for mTLS}\n  - {name: LOKI_CLIENT_KEY_PATH, purpose: client key for\
  \ mTLS}\n  - {name: LOKI_CA_CERT_PATH, purpose: server CA certificate}\nagent_note: >-\n  An agent must not assume a self-hosted Loki is protected. A Loki exposed without a fronting proxy\n  accepts unauthenticated reads and writes for any tenant it is asked for, which is the single most\n  important operational fact about this API.\ndocs:\n  - https://grafana.com/docs/loki/latest/reference/loki-http-api/\n  - https://grafana.com/docs/loki/latest/operations/authentication/\n  - https://grafana.com/docs/loki/latest/operations/multi-tenancy/\nchecked: '2026-08-27'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grafana-loki/refs/heads/main/authentication/grafana-loki-authentication.yml
summary_line: 6 schemes
tags:
- Company
- Logs
- Logging
- Log Aggregation
- Observability
- Monitoring
- Open-Source
- LogQL
- OpenTelemetry
- Telemetry
- Kubernetes
- Cloud-Native
---
