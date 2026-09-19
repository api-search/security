---
api_specs:
- filename: pagesnap-account-api-openapi.yml
  format: yaml
  label: Pagesnap Account API
  slug: pagesnap-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-account-api-openapi.yml
- filename: pagesnap-agents-api-openapi.yml
  format: yaml
  label: Pagesnap Agents API
  slug: pagesnap-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-agents-api-openapi.yml
- filename: pagesnap-billing-api-openapi.yml
  format: yaml
  label: Pagesnap Billing API
  slug: pagesnap-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-billing-api-openapi.yml
- filename: pagesnap-content-api-openapi.yml
  format: yaml
  label: Pagesnap Content API
  slug: pagesnap-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-content-api-openapi.yml
- filename: pagesnap-crawl-api-openapi.yml
  format: yaml
  label: Pagesnap Crawl API
  slug: pagesnap-crawl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-crawl-api-openapi.yml
- filename: pagesnap-diff-api-openapi.yml
  format: yaml
  label: Pagesnap Diff API
  slug: pagesnap-diff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-diff-api-openapi.yml
- filename: pagesnap-discovery-api-openapi.yml
  format: yaml
  label: Pagesnap Discovery API
  slug: pagesnap-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-discovery-api-openapi.yml
- filename: pagesnap-monitors-api-openapi.yml
  format: yaml
  label: Pagesnap Monitors API
  slug: pagesnap-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-monitors-api-openapi.yml
- filename: pagesnap-status-api-openapi.yml
  format: yaml
  label: Pagesnap Status API
  slug: pagesnap-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-status-api-openapi.yml
- filename: pagesnap-support-api-openapi.yml
  format: yaml
  label: Pagesnap Support API
  slug: pagesnap-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-support-api-openapi.yml
- filename: pagesnap-x402-api-openapi.yml
  format: yaml
  label: Pagesnap X402 API
  slug: pagesnap-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/openapi/pagesnap-x402-api-openapi.yml
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Pagesnap Trust Center
name_suffix: Trust Center
overview: Pagesnap maintains a public trust center covering its security and compliance posture.
provider_name: Pagesnap
provider_slug: pagesnap
slug: pagesnap-trust-center
source_filename: pagesnap-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://pagesnap.142-93-197-141.sslip.io/trust\nprobe:\n  url: https://pagesnap.142-93-197-141.sslip.io/trust\n  http_status: 200\ntitle: Trust & transparency\ncertifications: []\ncompliance_programs: []\ndisclaimer: >-\n  Quoted verbatim: \"Pagesnap is a small experimental service, not a compliance-certified\n  platform.\" No SOC 2, ISO 27001, PCI DSS, HIPAA, GDPR-certification or FedRAMP claim appears\n  anywhere on the site. This artifact records a trust CENTER, not a compliance posture.\noperator_disclosure:\n  model: AI-operated within a human owner's scope\n  detail: >-\n    AI coding and operations agents build, deploy, monitor, document and support the service. A\n    human owner supplied the account and single VPS, set product scope, and retains ultimate\n    control of the server and payment wallet. The agents \"are not a company officer or a\n    substitute for a human legal contact.\"\n  source_code: https://github.com/CalibratedGhosts/PageSnap\n\
  \  source_note: >-\n    Public for inspection; the README reserves all rights until the human owner selects a\n    software license. Public visibility is not a license grant.\ninfrastructure:\n  regions: 1 (New York City)\n  failover: none\n  sla: none\n  detail: >-\n    \"A host, network, process, browser, or operator failure can interrupt the whole service.\"\n    Process uptime on the stats page resets on deployment and is not service availability.\nsecurity_practices:\n  transport: HTTP redirects to HTTPS; HSTS max-age 63072000 with includeSubDomains and preload.\n  key_storage: >-\n    High-entropy keys shown once and stored server-side as SHA-256 hashes only. The keys and\n    dashboard pages save the raw key in the browser's localStorage - the provider flags this as a\n    risk for anyone with access to that browser profile.\n  key_transport: >-\n    Query-string authentication is a documented compatibility option the provider itself advises\n    against; use the Authorization header.\n\
  \  ssrf: >-\n    Only public HTTP(S) destinations accepted; DNS results and every redirect re-checked;\n    localhost, private, link-local, cloud-metadata and blocked hostnames refused. \"A valid public\n    URL can still return hostile content, so callers must treat output as untrusted.\"\n  render_isolation: >-\n    Fresh Playwright context per job, closed afterwards. No caller cookies or credentials are\n    accepted. Bounded by time, response size, concurrency and target-host limits. Described as\n    \"useful isolation, not a claim that Chromium or the host can never have a vulnerability.\"\n  cookies: Public pages and public APIs set no tracking or login cookie.\n  payment_verification: >-\n    After the x402 facilitator reports settlement, Pagesnap independently queries Base RPC\n    providers and checks a mined successful receipt plus the exact USDC Transfer contract, payer,\n    recipient, amount and signed nonce before releasing paid output.\nsecurity_reviews:\n  count: 3\n \
  \ date: '2026-09-02'\n  independent: false\n  disclaimer: >-\n    Quoted verbatim: \"They were conducted by the project agents and are not independent\n    penetration tests or certifications.\"\n  scope:\n    - Request boundaries, batch quota enforcement, bounded caches\n    - Free-plan quotas, internal-metric exclusion, invoice caps, ticket/admin CSRF, redaction, payment reorg handling\n    - Independent x402 receipt verification, A2A isolation, crawl persistence, receipt revalidation, embed URL boundary, research-job timeouts\ndata_handling:\n  sells_customer_data: false\n  detail: lifecycle/pagesnap-lifecycle.yml retention block carries the full published table.\n  caution: >-\n    The provider warns against putting secrets, credentials, personal data or signed URLs in\n    target URLs or support messages, and notes it cannot send outbound email so a lost raw key\n    cannot be recovered.\npublic_evidence:\n  - https://pagesnap.142-93-197-141.sslip.io/status\n  - https://pagesnap.142-93-197-141.sslip.io/v1/status\n\
  \  - https://pagesnap.142-93-197-141.sslip.io/stats\n  - https://pagesnap.142-93-197-141.sslip.io/log\n  - https://github.com/CalibratedGhosts/PageSnap\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/security/pagesnap-trust-center.yml
summary_line: trust center published
tags:
- Developer Tools
- Web Scraping
- web-to-markdown
- screenshot-api
- PDF Generation
- Metadata Extraction
- MCP
- A2A
- x402
- AI Agents
- Content Extraction
- Structured Data
- Web Crawling
- Change Monitoring
- llms-txt
- Agent Payments
- Software-as-a-Service
trust_url: ''
---
