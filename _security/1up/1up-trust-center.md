---
certification_count: 3
certifications:
- SOC 2 Type 2
- ISO 27001
- GDPR
description: ''
kind: trust-center
layout: security
name: 1Up Trust Center
name_suffix: Trust Center
overview: 1up maintains a public trust center documenting SOC 2 Type 2, ISO 27001, and GDPR compliance.
provider_name: 1up
provider_slug: 1up
slug: 1up-trust-center
source_filename: 1up-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nprobe: true\nsource: https://1up.ai/security\nurl: https://1up.ai/security\nnote: >-\n  1up has no trust portal in the Vanta/SafeBase/Drata sense — trust.1up.ai, 1up.ai/trust,\n  1up.ai/trust-center and 1up.ai/compliance all fail to resolve or return HTTP 404, and\n  1up.ai/llms.txt advertises a https://1up.ai/trust page that does not exist. What it does\n  publish is a \"Data Security & Privacy\" page carrying three compliance badges as images,\n  with no linked audit report, scope statement, audit period, auditor name or subprocessor\n  list behind them. The help centre's procurement article confirms the report exists but is\n  request-only: \"Your IT team might ask us to complete a security review or to provide a\n  SOC2 report.\" So: certifications are asserted publicly, artifacts are gated on sales\n  contact.\ncertifications:\n- SOC 2 Type 2\n- ISO 27001\n- GDPR\nevidence:\n- source: https://1up.ai/security\n  kind: badge-image\
  \ alt text\n  items:\n  - alt: AICPA SOC 2 Type 2 badge\n    file: 69e84a84370417c58517b139_soc-badge.svg\n  - alt: ISO 27001 badge\n    file: 69e84b90c348d1f4c490a461_iso-badge.avif\n  - alt: GDPR compliance badge\n    file: 69c379b42014b7a7f533371d_badge-03.svg\n- source: https://help.1up.ai/en/articles/12995986-pricing-and-procurement\n  kind: procurement guidance\n  quote: >-\n    Your IT team might ask us to complete a security review or to provide a SOC2 report.\n- source: https://help.1up.ai/en/articles/12997329-security-and-privacy-basics\n  kind: security controls\n  items:\n  - AES-256 encryption at rest\n  - AWS hosting with US / EU / AU data-residency choice\n  - per-workspace data isolation\n  - customer data never used to train models\nreport_access: request-only via sales / security review\ndead_pointer_finding: >-\n  https://1up.ai/llms.txt lists \"Trust / Security: https://1up.ai/trust\" among its\n  authoritative sources. That URL returns HTTP 404. The live page is https://1up.ai/security.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1up/refs/heads/main/security/1up-trust-center.yml
summary_line: SOC 2 Type 2, ISO 27001, GDPR
tags:
- Company
- Artificial Intelligence
- Sales Enablement
- Knowledge Management
- RFP Automation
- Security Questionnaires
- Model Context Protocol
- Agents
- SaaS
- Revenue Operations
trust_url: https://1up.ai/security
---
