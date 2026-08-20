---
certifications:
- ISO/IEC 42001
- SOC 2 Type II
- ISO 27001
- PCI DSS
- HIPAA
- GDPR
- TISAX
- CCPA
description: ''
kind: trust-center
layout: security
name: Cresta Trust Center
name_suffix: Trust Center
overview: Cresta maintains a public trust center documenting ISO/IEC 42001, SOC 2 Type II, ISO 27001, PCI DSS, HIPAA, GDPR, TISAX, and CCPA compliance.
provider_name: Cresta
provider_slug: cresta
slug: cresta-trust-center
source_filename: cresta-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://trust.cresta.com/\nurl: https://trust.cresta.com/\ntrust_page: https://cresta.com/trust\nplatform: SafeBase\ncertifications:\n- ISO/IEC 42001\n- SOC 2 Type II\n- ISO 27001\n- PCI DSS\n- HIPAA\n- GDPR\n- TISAX\n- CCPA\nevidence:\n- source: https://trust.cresta.com/\n  keywords:\n  - soc 2\n  - iso/iec 27001\n  - pci dss\n  - hipaa\n  - trust center\n  - gdpr\n- source: https://cresta.com/llm-info\n  fetched: '2026-08-14'\n  http_status: 200\n  claims: >-\n    \"Cresta is the first Customer Experience AI provider to achieve ISO/IEC\n    42001 certification — the international standard for responsible AI\n    management systems. Additional certifications and frameworks include SOC 2\n    Type II, HIPAA, GDPR, TISAX, CCPA, and PCI-DSS alignment.\"\n- source: https://cresta.com/blog/cresta-achieves-tisax-compliance\n  claims: TISAX compliance announcement.\n- source: https://cresta.com/.well-known/security.txt\n\
  \  claims: 'Policy: https://cresta.com/trust'\nnotes:\n- >-\n  Upgraded 2026-08-14 from Cresta's own first-party AI-facing page: added\n  ISO/IEC 42001, TISAX and CCPA, and split SOC 2 into SOC 2 Type II. PCI DSS is\n  stated by Cresta as *alignment*, not certification — retained in the list but\n  qualified in conformance/cresta-conformance.yml. If 0-working/\n  probe-security-programs.py is re-run it will flatten this list back to the\n  five keywords it can pattern-match on the SafeBase page; re-apply this file\n  rather than accept the regression.\n- >-\n  trust.cresta.com is a CNAMEd SafeBase tenant. Its /.well-known/\n  openid-configuration and oauth-authorization-server documents carry\n  \"issuer\": \"https://app.safebase.io/api/mcp\" and belong to SafeBase, not to\n  Cresta. See well-known/cresta-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cresta/refs/heads/main/security/cresta-trust-center.yml
summary_line: ISO/IEC 42001, SOC 2 Type II, ISO 27001, PCI DSS, HIPAA, GDPR, TISAX, CCPA
tags:
- Artificial Intelligence
- Contact Center
- Contact Center AI
- CCaaS
- Customer Experience
- Conversational AI
- Voice AI
- Agent Assist
- Conversation Intelligence
- Knowledge Agent
- Quality Management
- Real-Time Coaching
- After-Call Automation
- Enterprise AI
- MCP
- Customer Experience AI
- AI Agents
- gRPC
- Speech Analytics
- Enterprise Software
trust_url: https://trust.cresta.com/
---
