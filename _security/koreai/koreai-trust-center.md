---
api_specs:
- filename: Public-APIs
  format: yaml
  label: Kore.ai AI for Service Platform APIs
  slug: koreai-ai-for-service-platform-apis
  spec_type: Postman
  url: https://github.com/Koredotcom/Public-APIs
- filename: koreai-chat-api-openapi.yml
  format: yaml
  label: Kore.ai Chat API
  slug: koreai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koreai/refs/heads/main/openapi/koreai-chat-api-openapi.yml
- filename: koreai-conversation-api-openapi.yml
  format: yaml
  label: Kore.ai Conversation API
  slug: koreai-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koreai/refs/heads/main/openapi/koreai-conversation-api-openapi.yml
- filename: koreai-workflows-api-openapi.yml
  format: yaml
  label: Kore.ai Workflows API
  slug: koreai-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koreai/refs/heads/main/openapi/koreai-workflows-api-openapi.yml
certifications:
- SOC 2 Type 2
- PCI DSS
- ISO/IEC 27001:2022
- GDPR
- CCPA
- EU AI Act
- DESC Cloud Service Provider
description: ''
kind: trust-center
layout: security
name: Koreai Trust Center
name_suffix: Trust Center
overview: Kore.ai maintains a public trust center documenting SOC 2 Type 2, PCI DSS, ISO/IEC 27001:2022, GDPR, CCPA, EU AI Act, and DESC Cloud Service Provider compliance.
provider_name: Kore.ai
provider_slug: koreai
slug: koreai-trust-center
source_filename: koreai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://trust.kore.ai/\nurl: https://trust.kore.ai/\nplatform: SafeBase by Drata\naccess: >-\n  The index of documents and the certification list are public. The underlying reports and\n  policies are request-gated (NDA/approval), which is the normal SafeBase posture.\nprobe:\n  url: https://trust.kore.ai/\n  curl_status: 403\n  curl_note: >-\n    A plain curl with a browser User-Agent receives a Cloudflare interstitial\n    (\"Just a moment...\", noindex/nofollow). The page renders normally in a browser. This is\n    an edge bot policy, NOT a dead page — it is recorded as live.\n  browser_render_status: 200\n  checked: '2026-08-23'\ncertifications:\n- SOC 2 Type 2\n- PCI DSS\n- ISO/IEC 27001:2022\n- GDPR\n- CCPA\n- EU AI Act\n- DESC Cloud Service Provider\ndocument_categories:\n- Information Security Overview and Policy\n- Vulnerability Management Process and SLA Policy\n- Data Security (encryption at rest and in transit,\
  \ backups, customer data protection)\n- Secure Software Development Life Cycle\n- Responsible AI Framework\n- AI Transparency and Explainability (bias and hallucination monitoring)\n- Product security (SSO, RBAC, MFA)\n- Infrastructure and network security (firewall, anti-DDoS)\n- Business continuity and disaster recovery\n- Incident response and management\n- Security awareness and training policies\nlegal_and_commercial_documents:\n- Certificate of Liability Insurance\n- Enterprise Service Level Agreement\n- Platform License Agreement\nin_product_security_controls:\n  note: >-\n    Beyond the trust center, the platform ships customer-facing controls documented in the\n    release notes and admin docs — BYOK/KMS with Azure Key Vault and AWS, a selectable\n    KMS compliance level of GDPR / SOC2 / NIST enforced at configuration-write time, split\n    DEK-retirement and KEK-rewrap key rotation with preflight checks, PII protection,\n    guardrails, and a session-scoped encrypted secret\
  \ vault that keeps tool-returned\n    credentials out of the LLM context.\n  sources:\n  - https://docs.kore.ai/agent-platform/administration/security-observability-settings\n  - https://docs.kore.ai/agent-platform/pii-protection\n  - https://docs.kore.ai/agent-platform/release-notes/recent-updates\nvulnerability_disclosure:\n  public_policy: false\n  bug_bounty: false\n  note: >-\n    NO public vulnerability disclosure path was found. /.well-known/security.txt returns\n    404 on www.kore.ai, docs.kore.ai and agents.kore.ai and 403 on platform.kore.ai and\n    bots.kore.ai; no HackerOne, Bugcrowd or Intigriti program was found; and no\n    /security or /responsible-disclosure page exists (www.kore.ai/security returns 404).\n    The trust center lists a \"Vulnerability Management Process and SLA Policy\" document,\n    but that is an internal process description behind the request gate, not a route for an\n    outside researcher to report a finding. Because there is no public route, this\
  \ repo\n    emits no Security / VulnerabilityDisclosure pointer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koreai/refs/heads/main/security/koreai-trust-center.yml
summary_line: SOC 2 Type 2, PCI DSS, ISO/IEC 27001:2022, GDPR, CCPA, EU AI Act, DESC Cloud Service Provider
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Agents
- Agent Platform
- Contact Center
- Customer Experience
- Employee Experience
- Voice
- Automation
- Model Context Protocol
- Enterprise Software
trust_url: https://trust.kore.ai/
---
