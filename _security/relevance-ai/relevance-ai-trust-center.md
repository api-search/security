---
api_specs:
- filename: relevance-ai-openapi.json
  format: json
  label: Relevance AI API
  slug: relevance-ai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relevance-ai/refs/heads/main/openapi/relevance-ai-openapi.json
certifications:
- SOC 2 Type II
- GDPR
description: ''
kind: trust-center
layout: security
name: Relevance Ai Trust Center
name_suffix: Trust Center
overview: Relevance AI maintains a public trust center documenting SOC 2 Type II and GDPR compliance.
provider_name: Relevance AI
provider_slug: relevance-ai
slug: relevance-ai-trust-center
source_filename: relevance-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://trust.relevanceai.com/, https://relevanceai.com/docs/admin/security,\n  https://relevanceai.com/enterprise, https://relevanceai.com/data-security-policy\nprovider: Relevance AI\nproviderId: relevance-ai\ntrust_center:\n  url: https://trust.relevanceai.com/\n  status: 200\n  platform: Vanta Trust Report\n  machine_readable: false\n  note: >-\n    The page is a Vanta-hosted trust report rendered entirely client-side; every /api/* path on\n    the host returns the same SPA shell, so no machine-readable certification list can be read\n    from it. The certifications below are taken from the provider's own security overview,\n    enterprise page and pricing feature matrix, which state them in text.\ncertifications:\n  - name: SOC 2 Type II\n    body: AICPA\n    status: current\n    scope: platform\n    evidence:\n      - https://relevanceai.com/docs/admin/security\n      - https://relevanceai.com/enterprise\n     \
  \ - https://relevanceai.com/llms.txt\n  - name: GDPR\n    status: compliant\n    evidence:\n      - https://relevanceai.com/docs/admin/security\n      - https://relevanceai.com/docs/get-started/pricing\nnot_claimed:\n  - ISO 27001\n  - PCI DSS\n  - HIPAA\n  - FedRAMP\n  - ISO 42001\nsecurity_program:\n  data_residency:\n    regions: [United States, Europe, Australia]\n    detail: A project is deployed to one region; the API host encodes it (api-{region}.stack.tryrelevance.com).\n  tenant_isolation: documented\n  encryption:\n    at_rest: true\n    in_transit: true\n    customer_managed_keys: documented\n  access_management:\n    sso_saml: Enterprise\n    rbac: Enterprise\n    audit_logs: Enterprise\n  ai_specific_controls:\n    - PII masking / redaction (Presidio-powered, Enterprise)\n    - Prompt-injection detection recorded on the invoke_agent span (Enterprise)\n    - Human-in-the-loop approval gates\n    - Work hour controls\n  vulnerability_management: >-\n    \"Our infrastructure\
  \ is continuously scanned for vulnerabilities and patched within strict\n    SLAs.\" No SLA figure is published.\n  third_party_assessments: Performed by independent security firms; reports available to Enterprise customers under NDA.\n  security_questionnaire: Available via the trust center / sales.\n  policies:\n    data_security_policy: https://relevanceai.com/data-security-policy\n    privacy_policy: https://relevanceai.com/privacy-policy\n    terms: https://relevanceai.com/terms-and-conditions\nvulnerability_disclosure:\n  program_found: false\n  security_txt: false\n  bug_bounty: false\n  probed:\n    - url: https://relevanceai.com/.well-known/security.txt\n      status: 404\n    - url: https://docs.relevanceai.com/.well-known/security.txt\n      status: 404\n    - url: https://mcp.relevanceai.com/.well-known/security.txt\n      status: 404\n    - url: https://relevanceai.com/security\n      status: 404\n  detail: >-\n    No RFC 9116 security.txt, no published disclosure policy page,\
  \ and no HackerOne / Bugcrowd\n    / Intigriti program was found. There is no documented channel for reporting a\n    vulnerability other than general support. Recorded as an honest absence — no\n    VulnerabilityDisclosure or Security pointer is emitted, because none is served.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relevance-ai/refs/heads/main/security/relevance-ai-trust-center.yml
summary_line: SOC 2 Type II, GDPR
tags:
- AI Agents
- AI Automation
- Multi-Agent Systems
- Agent Platform
- MCP
- agent-native
- Workflow-Automation
- LLM Orchestration
- Knowledge-Management
- Observability
- Sales Automation
- GTM Engineering
trust_url: ''
---
