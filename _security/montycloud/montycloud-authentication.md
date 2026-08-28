---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Montycloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: MontyCloud declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: MontyCloud
provider_slug: montycloud
scheme_count: 3
schemes:
- description: API key issued to a user inside the DAY2 platform.
  id: apiKeyHeader
  in: header
  name: x-api-key
  required: true
  type: apiKey
- description: The API secret key, sent raw in the Authorization header. It is NOT an RFC 6750 bearer token and carries no scheme prefix — the SDK assigns the secret directly (headers["Authorization"] = credentials.secret_key).
  id: apiSecretHeader
  in: header
  name: Authorization
  required: true
  type: apiKey
- description: Selects the tenant a request executes against. Set by Session.set_tenant() / the CLI tenant context. Omitting it uses the caller's default tenant; most resource paths also take the tenant id as a path parameter.
  id: tenantContext
  in: header
  name: x-tenant-id
  required: false
  type: apiKey
slug: montycloud-authentication
source_filename: montycloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: >-\n  pypi:day2@0.5.0 (day2/client/base.py, day2/auth/credentials.py) +\n  https://montycloud.com/mcp-server-security-statement/ + https://montycloud.com/trust-center/\nnote: >-\n  MontyCloud publishes no public OpenAPI and no public authentication reference page — the\n  developer docs at developer.montycloud.com are a private GitHub Pages site that 302s to a GitHub\n  organization login. This profile is derived from MontyCloud's own published Python SDK\n  (`day2` 0.5.0 on PyPI) and corroborated by two first-party prose documents: the MCP Server\n  Security Statement and the Trust Center.\nsummary: >-\n  Paired-secret API authentication. Every DAY2 API request carries an API key in `x-api-key` and\n  the API secret key in `Authorization`; tenant scope is selected per request with `x-tenant-id`.\n  There is no OAuth 2.0 flow, no bearer token exchange, and no published scope vocabulary on the\n  product API — authorization is\
  \ DAY2 platform RBAC attached to the user the key was minted for.\nschemes:\n  - id: apiKeyHeader\n    type: apiKey\n    in: header\n    name: x-api-key\n    required: true\n    description: API key issued to a user inside the DAY2 platform.\n  - id: apiSecretHeader\n    type: apiKey\n    in: header\n    name: Authorization\n    required: true\n    description: >-\n      The API secret key, sent raw in the Authorization header. It is NOT an RFC 6750 bearer token\n      and carries no scheme prefix — the SDK assigns the secret directly\n      (headers[\"Authorization\"] = credentials.secret_key).\n  - id: tenantContext\n    type: apiKey\n    in: header\n    name: x-tenant-id\n    required: false\n    description: >-\n      Selects the tenant a request executes against. Set by Session.set_tenant() / the CLI tenant\n      context. Omitting it uses the caller's default tenant; most resource paths also take the\n      tenant id as a path parameter.\ncredential_sources:\n  - inline constructor\
  \ arguments (api_key, api_secret_key)\n  - environment variables DAY2_API_KEY and DAY2_API_SECRET_KEY\n  - profile config file ~/.day2/config, written by `day2 auth configure`\nidentity_provider:\n  service: Amazon Cognito\n  gateway: AWS API Gateway\n  source: https://montycloud.com/mcp-server-security-statement/\n  note: >-\n    MontyCloud states the same API Gateway + Cognito framework fronts both the core API services\n    and the CloudOps MCP Server, and that MCP access uses the same API key + secret key pair.\nauthorization:\n  model: rbac\n  scope_vocabulary: none-published\n  detail: >-\n    Permissions granted by an API key are those of the DAY2 user identity it was generated for,\n    under a stated principle of least privilege. RBAC governs every platform feature and enforces\n    tenant isolation; MontyCloud publishes no OAuth scope list, so scopes/ is intentionally absent\n    from this repo rather than fabricated.\n  source: https://montycloud.com/mcp-server-security-statement/\n\
  end_user_sso:\n  supported: true\n  protocols:\n    - SAML 2.0\n    - Azure Active Directory / Entra ID\n  scope: DAY2 platform console sign-in (app.montycloud.com), not API credentials\n  docs: https://support.montycloud.com/support/solutions/articles/62000206236-single-sign-on-in-day2-overview-\ncloud_account_trust:\n  mechanism: AWS cross-account IAM role with a unique per-customer external ID\n  detail: >-\n    MontyCloud accesses customer AWS accounts through a scoped cross-account IAM role limited to\n    resource metadata (names, tag key/values) and CloudTrail log streams. The role is assumable\n    only by MontyCloud's designated AWS account IDs. No MontyCloud employee holds direct customer\n    account access. Temporary IAM access keys are held in application memory only and are never\n    stored or logged.\n  source: https://montycloud.com/trust-center/\n  docs: https://support.montycloud.com/support/solutions/articles/62000213248-day2-aws-iam-permissions\ntransport:\n  tls_required:\
  \ true\n  note: All data in transit encrypted with TLS; at rest with AES-256 (Trust Center).\nfailure_modes:\n  - status: 401\n    meaning: authentication failed (SDK raises AuthenticationError)\n  - status: 403\n    meaning: authenticated but not permitted (SDK also raises AuthenticationError)\nmcp_authentication:\n  endpoint: https://api.montycloud.com/mcp\n  model: api-key-and-secret\n  observed: anonymous tools/list POST returns HTTP 401 {\"message\":\"Unauthorized\"}\n  probed: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/montycloud/refs/heads/main/authentication/montycloud-authentication.yml
summary_line: 3 schemes
tags:
- Cloud
- Cloud Operations
- Managed Service Providers
- Governance
- Compliance
- Cost Management
- Artificial Intelligence
- Agents
- Model Context Protocol
- Multi-Tenant
- Infrastructure
---
