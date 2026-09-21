---
api_specs:
- filename: fodda-ai-openapi.yml
  format: yaml
  label: Fodda Context & Research API
  slug: fodda-context-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fodda-ai/refs/heads/main/openapi/fodda-ai-openapi.yml
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Fodda Ai Trust Center
name_suffix: Trust Center
overview: Fodda (PSFK) maintains a public trust center covering its security and compliance posture.
provider_name: Fodda (PSFK)
provider_slug: fodda-ai
slug: fodda-ai-trust-center
source_filename: fodda-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://www.fodda.ai/compliance-dossier + https://www.fodda.ai/iso-42001-compliance + https://www.fodda.ai/security\n  + https://www.fodda.ai/blog/security-refresh-2026 + fodda-mcp SECURITY_SUMMARY.md / SECURITY_PACK.md\nchecked: '2026-09-19'\nsummary: 'Fodda publishes a procurement-facing \"Compliance Dossier — MCP Server & API Governance\" (tool surface\n  and write capability, data handling and training use, authentication and credential scope, assurance position,\n  security contacts; last updated 2026-08-27) and an ISO/IEC 42001 alignment page with an Annex A control mapping.\n  No certification is held or claimed: the assurance position is ALIGNMENT with ISO/IEC 42001:2023 and NIST AI RMF,\n  a NIST CSF 2.0-aligned program, and a SOC 2 Type II readiness roadmap for Q4 2026; the only SOC 2 report cited\n  is Clerk''s (the delegated identity provider). Recorded as a published compliance program without certifications\n\
  \  — the Compliance pointer rests on the program, the TrustCenter pointer on the dossier.'\nportal:\n  url: https://www.fodda.ai/compliance-dossier\n  provider: self-hosted page\n  last_updated: '2026-08-27'\n  audience: InfoSec and IT procurement teams\n  sections:\n  - 1. Tool Surface & Write Capability\n  - 2. Data Handling & Training Use\n  - 3. Authentication & Credential Scope\n  - 4. Assurance Position & Governance\n  - 5. Security Contacts\ncertifications_held: []\nalignment_claims:\n- framework: ISO/IEC 42001:2023\n  status: alignment (not certified)\n  url: https://www.fodda.ai/iso-42001-compliance\n  last_updated: '2026-08-27'\n  evidence: 'Annex A control mapping: A.5 AI System Life Cycle (read-only tool contracts, deterministic execution);\n    A.6 Data for AI Systems (usage logging ledger, zero model training on client queries); A.7 Information for Interested\n    Parties (provenance & evidence chain); A.8 Responsible Use (automated behavioral test checks); A.9 Third Parties\n\
  \    (graceful model degradation error bounds).'\n- framework: NIST AI RMF\n  status: alignment\n  url: https://www.fodda.ai/compliance-dossier\n- framework: NIST CSF 2.0\n  status: program aligned\n  url: https://www.fodda.ai/blog/security-refresh-2026\n  date: '2026-02-12'\n- framework: SOC 2 Type II\n  status: readiness roadmap — target Q4 2026\n  url: https://www.fodda.ai/blog/security-refresh-2026\ndelegated_assurance:\n- vendor: Clerk\n  role: identity / authorization server (clerk.fodda.ai)\n  claim: no password custody, SOC 2 Type 2 held since May 2022\n  source: https://www.fodda.ai/compliance-dossier\n- vendor: Google Cloud Platform\n  role: 'hosting (Cloud Run / App Engine — server: Google Frontend)'\n  source: https://www.fodda.ai/blog/security-refresh-2026\n- vendor: Stripe\n  role: payments and Shared Payment Tokens\n  source: https://www.fodda.ai/llms.txt\ndata_handling:\n  retention: Query text retained in an internal usage ledger for 12 months for billing and telemetry,\
  \ then purged;\n    result text is not retained.\n  training: Zero model training on client data.\n  options: Zero-retention query logging (in-memory execution), pseudonymous identifiers, and 30-day termination\n    purge available as standard/negotiated contract options.\n  isolation: Per-graph and per-tenant isolation enforced at the API layer (SECURITY_SUMMARY.md); tenant isolation\n    architecture (blog).\n  encryption: TLS 1.2+ in transit (SECURITY_SUMMARY.md); TLS 1.3 observed (security/fodda-ai-domain-security.yml).\n  deployment_options: 'Model B: MCP proxy hosted in the customer''s own Google Cloud project; /enterprises advertises\n    air-gapped on-premise deployments.'\ncontacts:\n  security: security@fodda.ai\n  compliance: compliance@fodda.ai\n  privacy: privacy@fodda.ai\n  legal: legal@fodda.ai\nrelated_documents:\n- name: Security & Procurement Summary\n  url: https://github.com/piers-fawkes/fodda-mcp/blob/main/SECURITY_SUMMARY.md\n- name: Security Pack\n  url: https://github.com/piers-fawkes/fodda-mcp/blob/main/SECURITY_PACK.md\n\
  - name: Enterprise MCP Setup\n  url: https://github.com/piers-fawkes/fodda-mcp/blob/main/Enterprise_MCP_Setup.md\npointer_basis: 'TrustCenter: the dossier is a real procurement-facing governance page. Compliance: a published,\n  framework-mapped compliance program (ISO 42001 Annex A, NIST) — NOT a certification; readers should not infer\n  SOC 2 / ISO certification from the pointer.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fodda-ai/refs/heads/main/security/fodda-ai-trust-center.yml
summary_line: trust center published
tags:
- Market Intelligence
- Trend Research
- Knowledge Graph
- Consumer Insights
- Earnings Intelligence
- Brand Intelligence
- Research
- Institutional Data
- MCP
- A2A
- agent-native
- Machine Payments
- Company
trust_url: ''
---
