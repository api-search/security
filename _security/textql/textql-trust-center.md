---
api_specs:
- filename: textql-v2-openapi.yml
  format: yaml
  label: TextQL v2 API
  slug: textql-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/openapi/textql-v2-openapi.yml
- filename: textql-chat-v1-openapi.yml
  format: yaml
  label: TextQL Platform API (v1)
  slug: textql-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/openapi/textql-chat-v1-openapi.yml
- filename: textql-platform-api-openapi.yml
  format: yaml
  label: TextQL Public RPC API
  slug: textql-public-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/openapi/textql-platform-api-openapi.yml
certifications:
- SOC 2 Type II
- HIPAA
- GDPR
- SOX
description: ''
kind: trust-center
layout: security
name: Textql Trust Center
name_suffix: Trust Center
overview: TextQL maintains a public trust center documenting SOC 2 Type II, HIPAA, GDPR, and SOX compliance.
provider_name: TextQL
provider_slug: textql
slug: textql-trust-center
source_filename: textql-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://textql.com/security\nurl: https://trust.textql.com/\ntrust_center:\n  url: https://trust.textql.com/\n  platform: Drata\n  redirects_to: https://app.drata.com/trust/36f9232d-d1fa-4cc8-ac65-746a94a71cc3\n  probed: '2026-08-30'\n  http_status: 403\n  readable: false\n  note: >-\n    The trust center is linked from textql.com/security as \"Visit Trust Center\" and resolves to a\n    Drata-hosted portal, but returned 403 to both a browser-User-Agent curl and a WebFetch. Its\n    contents could not be read this run. The certifications below are therefore taken from TextQL's\n    OWN security page, which was fetched successfully, rather than from the portal.\ncertifications:\n- name: SOC 2 Type II\n  source: https://textql.com/security\n  detail: Audited annually, report on request.\n- name: HIPAA\n  source: https://textql.com/security\n  detail: BAAs signed; PHI never leaves the customer's cloud. Enterprise tier.\n- name:\
  \ GDPR\n  source: https://textql.com/security\n  detail: DPA available, EU data residency.\n- name: SOX\n  source: https://textql.com/pricing\n  detail: >-\n    Listed in the Enterprise tier's compliance column as \"SOX, audit & policy support\" — a support\n    posture for the customer's own SOX programme, not a certification TextQL holds.\n  qualifier: support-posture-not-certification\ncorrections:\n  - >-\n    An earlier automated pass recorded ISO 27001 from a keyword match on the Drata portal URL. That\n    claim is REMOVED — the portal returned 403 and was never read, and ISO 27001 appears nowhere on\n    TextQL's own security or pricing pages. Only SOC 2 Type II, HIPAA and GDPR are provider-stated.\nsecurity_posture:\n  source: https://textql.com/security\n  probed: '2026-08-30'\n  http_status: 200\n  model: >-\n    \"TextQL treats its own agent as an untrusted principal. Every query clears four gates — identity,\n    entitlement, execution, audit — before a byte of your data moves.\"\
  \n  isolation: gVisor sandbox per session, destroyed when the session ends; no sharing between customers or between two users of the same customer\n  encryption: TLS 1.2+ in transit, AES-256 at rest, customer-managed keys via customer KMS on VPC and on-prem installs\n  deployment_options: [multi-tenant SaaS, single-tenant, customer VPC, BYOC, on-premises, air-gapped, private link]\n  model_training: >-\n    \"Never trained on your data — not our models, not a provider's, with no contractual carve-out.\"\n    Customers may bring their own Bedrock, Vertex or Azure OpenAI deployment so inference never leaves\n    their account.\n  identity: SAML 2.0 and OIDC (IdP- and SP-initiated), JIT provisioning, SCIM 2.0 lifecycle, domain claim enforcement, MFA enforced at the customer IdP\n  authorization: >-\n    Roles compose from named grants and resolve per request rather than at login. Row filters and\n    column masks are evaluated by the customer's warehouse — Snowflake row access policies, Unity\n\
  \    Catalog column masks, BigQuery policy tags — so revoking a grant upstream takes effect on the next\n    query.\n  network: gVisor-isolated sandbox per run, outbound domain allowlist, credential-injecting egress proxy, PrivateLink/VPC peering/static egress IPs on enterprise\n  secrets: Credentials live in a vault the agent process cannot read.\n  audit: Audit Log (AuditLogService in the Public RPC API) covers security and administrative activity\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/security/textql-trust-center.yml
summary_line: SOC 2 Type II, HIPAA, GDPR, SOX
tags:
- Company
- Artificial Intelligence
- Analytics
- Business Intelligence
- Data
- Agents
- MCP
- Semantic Layer
- Text-to-SQL
- Data Warehouse
- Enterprise
trust_url: https://trust.textql.com/
---
