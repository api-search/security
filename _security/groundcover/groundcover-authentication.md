---
api_key_in: []
auth_types: []
description: 'groundcover issues four distinct credential types, each scoped to a different surface. There is no single "API token": a key that reads data cannot ingest it, and a key that ingests cannot read. Derived from documentation rather than a spec — groundcover publishes no OpenAPI, so no securitySchemes block exists to parse.'
kind: authentication
layout: security
method: searched
name: Groundcover Authentication
name_suffix: Authentication
oauth_flows: []
overview: Groundcover declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Groundcover
provider_slug: groundcover
scheme_count: 5
schemes:
- applies_to:
  - https://api.groundcover.com
  - https://mcp.groundcover.com/api/mcp
  - Terraform / Pulumi / Crossplane providers
  - Official Go, Python and TypeScript SDKs (env GC_API_KEY)
  binding: Every API key is tied to one service account and inherits that account's RBAC policies. A key may optionally be limited to a subset of those policies; it can never exceed the parent service account's permissions.
  docs: https://docs.groundcover.com/use-groundcover/remote-access-and-apis/api-keys
  format: 'Authorization: Bearer <YOUR_API_KEY>'
  header: Authorization
  id: api-key-bearer
  in: header
  lifecycle:
    created_by: Admins only, in Settings -> Access -> API Keys
    expiry: none — keys do not expire automatically
    revealed: once, at creation
    revocation: immediate on revoke
  name: API Key (service-account bearer token)
  purpose: Read data and manage platform resources via REST.
  scheme: bearer
  type: http
- applies_to:
  - the tenant's BYOC ingestion endpoint (OTLP/HTTP and other data-source exporters)
  docs: https://docs.groundcover.com/use-groundcover/remote-access-and-apis/ingestion-keys
  header: apikey
  id: ingestion-key
  in: header
  name: Ingestion Key
  properties:
    lifetime: tied to the integration lifecycle
    permissions: write-only, plus optional remote-config read
    revealable: always
  purpose: Write-only — let sensors, integrations and browsers send telemetry to the backend.
  type: apiKey
- applies_to:
  - https://ds.groundcover.com
  deprecated: true
  docs: https://docs.groundcover.com/use-groundcover/remote-access-and-apis/querying-you-data-using-an-api
  header: X-ClickHouse-Key
  id: datasource-key
  in: header
  name: Datasource (ds) API Key — LEGACY
  obtained_via: groundcover auth get-datasources-api-key
  purpose: Connect to groundcover as a datasource and execute SQL directly against ClickHouse / VictoriaMetrics. Documented as deprecated but still present in older setups.
  type: apiKey
- docs: https://docs.groundcover.com/use-groundcover/remote-access-and-apis/build-alerts-and-dashboards-with-grafana-terraform-provider
  id: grafana-service-account-token
  name: Grafana Service Account Token
  purpose: Remotely create Grafana alerts and dashboards via the Grafana Terraform provider.
  type: apiKey
- applies_to:
  - https://mcp.groundcover.com/api/mcp
  authorization_endpoint: https://mcp.groundcover.com/mcp-oauth/authorize
  dynamic_client_registration: true
  evidence: RFC 8414 metadata at https://mcp.groundcover.com/.well-known/oauth-authorization-server (HTTP 200, probed 2026-08-29) and RFC 9728 metadata at /.well-known/oauth-protected-resource (200).
  flow: authorization_code
  id: mcp-oauth
  name: MCP OAuth 2.1
  pkce: S256
  purpose: Browser-login flow for agents connecting to the remote MCP server.
  registration_endpoint: https://mcp.groundcover.com/register-client
  revocation_endpoint: https://auth.groundcover.com/oauth/revoke
  scopes:
  - access:router
  token_endpoint: https://mcp.groundcover.com/mcp-oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: groundcover-authentication
source_filename: groundcover-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://docs.groundcover.com/use-groundcover/remote-access-and-apis\ndocs: https://docs.groundcover.com/use-groundcover/remote-access-and-apis/api-keys\nprovider: Groundcover\nproviderId: groundcover\ndescription: >-\n  groundcover issues four distinct credential types, each scoped to a different surface. There is no\n  single \"API token\": a key that reads data cannot ingest it, and a key that ingests cannot read.\n  Derived from documentation rather than a spec — groundcover publishes no OpenAPI, so no\n  securitySchemes block exists to parse.\nschemes:\n  - id: api-key-bearer\n    type: http\n    scheme: bearer\n    name: API Key (service-account bearer token)\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer <YOUR_API_KEY>'\n    applies_to:\n      - https://api.groundcover.com\n      - https://mcp.groundcover.com/api/mcp\n      - Terraform / Pulumi / Crossplane providers\n      - Official Go,\
  \ Python and TypeScript SDKs (env GC_API_KEY)\n    purpose: Read data and manage platform resources via REST.\n    binding: >-\n      Every API key is tied to one service account and inherits that account's RBAC policies. A key\n      may optionally be limited to a subset of those policies; it can never exceed the parent\n      service account's permissions.\n    lifecycle:\n      created_by: Admins only, in Settings -> Access -> API Keys\n      revealed: once, at creation\n      expiry: none — keys do not expire automatically\n      revocation: immediate on revoke\n    docs: https://docs.groundcover.com/use-groundcover/remote-access-and-apis/api-keys\n  - id: ingestion-key\n    type: apiKey\n    in: header\n    header: apikey\n    name: Ingestion Key\n    applies_to:\n      - the tenant's BYOC ingestion endpoint (OTLP/HTTP and other data-source exporters)\n    purpose: Write-only — let sensors, integrations and browsers send telemetry to the backend.\n    properties:\n      permissions:\
  \ write-only, plus optional remote-config read\n      revealable: always\n      lifetime: tied to the integration lifecycle\n    docs: https://docs.groundcover.com/use-groundcover/remote-access-and-apis/ingestion-keys\n  - id: datasource-key\n    type: apiKey\n    in: header\n    header: X-ClickHouse-Key\n    name: Datasource (ds) API Key — LEGACY\n    applies_to:\n      - https://ds.groundcover.com\n    purpose: >-\n      Connect to groundcover as a datasource and execute SQL directly against ClickHouse /\n      VictoriaMetrics. Documented as deprecated but still present in older setups.\n    obtained_via: 'groundcover auth get-datasources-api-key'\n    deprecated: true\n    docs: https://docs.groundcover.com/use-groundcover/remote-access-and-apis/querying-you-data-using-an-api\n  - id: grafana-service-account-token\n    type: apiKey\n    name: Grafana Service Account Token\n    purpose: Remotely create Grafana alerts and dashboards via the Grafana Terraform provider.\n    docs: https://docs.groundcover.com/use-groundcover/remote-access-and-apis/build-alerts-and-dashboards-with-grafana-terraform-provider\n\
  \  - id: mcp-oauth\n    type: oauth2\n    name: MCP OAuth 2.1\n    flow: authorization_code\n    pkce: S256\n    dynamic_client_registration: true\n    authorization_endpoint: https://mcp.groundcover.com/mcp-oauth/authorize\n    token_endpoint: https://mcp.groundcover.com/mcp-oauth/token\n    revocation_endpoint: https://auth.groundcover.com/oauth/revoke\n    registration_endpoint: https://mcp.groundcover.com/register-client\n    token_endpoint_auth_methods_supported: [none]\n    scopes:\n      - access:router\n    applies_to:\n      - https://mcp.groundcover.com/api/mcp\n    purpose: Browser-login flow for agents connecting to the remote MCP server.\n    evidence: >-\n      RFC 8414 metadata at https://mcp.groundcover.com/.well-known/oauth-authorization-server (HTTP\n      200, probed 2026-08-29) and RFC 9728 metadata at /.well-known/oauth-protected-resource (200).\nrouting_headers:\n  - name: X-Backend-Id\n    required: only for accounts associated with more than one backend\n    purpose:\
  \ Route the request to the correct backend.\n    where_to_find: Settings -> Access -> API Keys tab (section header)\n  - name: X-Tenant-UUID\n    required: false\n    purpose: Pin an MCP OAuth connection to a single workspace.\n  - name: X-Timezone\n    required: false\n    purpose: IANA time zone for relative time-window resolution (MCP).\nauthorization:\n  model: RBAC (policies + service accounts)\n  availability: Enterprise plan\n  permission_levels: [Admin, Editor, Viewer]\n  data_scope_modes:\n    - name: Simple\n      logic: AND across conditions, same scope for every entity type\n    - name: Advanced\n      logic: separate scope per data type (workload/infrastructure, logs, traces, events, metrics), OR within each\n  merging: >-\n    A user assigned multiple policies gets the HIGHEST permission level across them and the UNION\n    (OR) of their data scopes.\n  default_policies: [Default Admin Policy, Default Editor Policy, Default Viewer Policy]\n  docs: https://docs.groundcover.com/use-groundcover/role-based-access-control-rbac\n\
  notes:\n  - >-\n    API keys are only valid for the environment that issued them. Self-hosted (onPrem / airGapped)\n    deployments use their own API URL and their own keys.\n  - >-\n    Documented best practices: store in a secrets manager, assign least-privilege policies, rotate\n    periodically, revoke stale keys. A spike in 403 PERMISSION_DENIED usually means a revoked or\n    expired key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groundcover/refs/heads/main/authentication/groundcover-authentication.yml
summary_line: 5 schemes
tags:
- AIOps
- Observability
- Kubernetes
- eBPF
- Monitoring
- Logs
- Traces
- Metrics
- OpenTelemetry
- MCP
---
