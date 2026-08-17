---
certifications:
- SOC 2 Type 1
- SOC 2 Type 2
- SOC 3
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Chatsimple Trust Center
name_suffix: Trust Center
overview: Chatsimple maintains a public trust center documenting SOC 2 Type 1, SOC 2 Type 2, SOC 3, GDPR, and CCPA compliance.
provider_name: Chatsimple
provider_slug: chatsimple
slug: chatsimple-trust-center
source_filename: chatsimple-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://trust.expertise.ai/\nurl: https://trust.expertise.ai/\nsecurity_page: https://www.expertise.ai/security\nreview_request: >-\n  The security page offers a \"Start a security review\" path and a \"View Trust\n  Center\" link. There is NO vulnerability-disclosure or bug-bounty program: no\n  security.txt on any host, no security@ address, no responsible-disclosure\n  page, and no HackerOne/Bugcrowd/Intigriti listing. security/\n  chatsimple-vulnerability-disclosure.yml is therefore deliberately not written\n  and no `Security` pointer is wired in apis.yml.\ncertifications:\n- SOC 2 Type 1\n- SOC 2 Type 2\n- SOC 3\n- GDPR\n- CCPA\nreports:\n- Network Diagram\n- Pentest Report\n- BCP/DRP\nlegal:\n- Data Processing Agreement\n- Subprocessors\n- Cyber Insurance\nsecurity_controls:\n- RS256 token-based authentication with automatic expiry\n- Secure HTTP-only cookies and short-lived session tokens\n- 60-second expiring\
  \ presigned URLs for file access\n- HTTPS with HSTS and Content Security Policy (CSP)\n- Hashed API keys and HMAC webhook signatures\n- Vector database isolation per chatbot\n- AWS Secrets Manager for credential storage\n- Alignment with OWASP Top 10\nevidence:\n- source: https://trust.expertise.ai/\n  keywords:\n  - trust center\n  - soc 2 type 1\n  - soc 2 type 2\n  - soc 3\n- source: https://www.expertise.ai/security\n  keywords:\n  - gdpr\n  - ccpa\n  - aicpa soc\n- source: https://www.expertise.ai/security\n  fetched: '2026-08-13'\n  http_status: 200\n  keywords:\n  - soc 2 type ii\n  - soc 3\n  - independent penetration test\n  - dpa available\n- source: https://www.expertise.ai/changelog\n  fetched: '2026-08-13'\n  http_status: 200\n  keywords:\n  - 'SOC 2 Type II Compliance Achieved (changelog entry dated 2025-07-29)'\nproduct_security_model:\n  source: https://www.expertise.ai/security\n  fetched: '2026-08-13'\n  note: >-\n    The security page splits controls by product because\
  \ the two threat models\n    differ. Captured verbatim in summary because it is unusually specific for\n    this size of company and it is the provider's own published claim.\n  expertise_live:\n  - Tenant-scoped knowledge in an isolated vector namespace per chatbot/customer\n  - Untrusted-input boundaries between visitor messages, retrieved content and system instructions\n  - Input validation, rate limiting, spam controls and SSRF protections; output sanitization and embed restrictions\n  - Retrieval/response grounding controls\n  - Webhook signature checks, verification tokens and event deduplication on supported inbound channels\n  expertise_assistant:\n  - Skill-bundle screening of instructions, metadata, accessory files and declared connectors\n  - User-scoped microVM sandboxes with runtime, filesystem and process boundaries\n  - Backend-held connector credentials kept out of prompts; sandbox receives only scoped session credentials\n  - Deterministic server-side connector/method/route\
  \ authorization independent of model output\n  - Human approval required for classified writes; unknown write behaviour fails closed to review\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatsimple/refs/heads/main/security/chatsimple-trust-center.yml
summary_line: SOC 2 Type 1, SOC 2 Type 2, SOC 3, GDPR, CCPA
tags:
- Company
- AI Agents
- Conversational AI
- Chatbot
- Lead Generation
- Sales Automation
- CRM Integration
- Voice AI
- Go-To-Market
- Customer Engagement
trust_url: https://trust.expertise.ai/
---
