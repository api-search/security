---
certifications:
- SOC 2 Type II
- ISO 27001
- ISO 42001
- HIPAA
- GDPR
description: ''
kind: trust-center
layout: security
name: Deepip Trust Center
name_suffix: Trust Center
overview: DeepIP maintains a public trust center documenting SOC 2 Type II, ISO 27001, ISO 42001, HIPAA, and GDPR compliance.
provider_name: DeepIP
provider_slug: deepip
slug: deepip-trust-center
source_filename: deepip-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nprobe: true\nsource: https://trust.deepip.ai/\nurl: https://trust.deepip.ai/\nplatform: Vanta\ncertifications:\n- SOC 2 Type II\n- ISO 27001\n- ISO 42001\n- HIPAA\n- GDPR\nframeworks:\n- name: \"\\xA7203 StGB\"\n  note: German criminal-code professional-secrecy obligation, relevant to patent attorneys.\n- name: NIST 800-53 Moderate\n  note: Security policies stated to adhere to this baseline.\n- name: NIST Cybersecurity Framework (CSF)\ncontrols:\n  encryption_in_transit: TLS 1.2+\n  encryption_at_rest: AES-256\n  data_retention: >-\n    Zero data retention. Customer data is not stored by DeepIP's model providers\n    and is not used for training or fine-tuning; Microsoft's abuse monitoring is\n    disabled under DeepIP's Azure agreement.\n  hosting: Microsoft Azure, U.S.-based (EU and US regional stacks per status page)\n  tenancy: Complete segregation of users and organizational data\n  deployment_options: [cloud, on-premise]\nevidence:\n\
  - source: https://trust.deepip.ai/\n  status: 200\n  keywords: [soc 2 type ii, iso 27001, trust center, gdpr]\n- source: https://www.deepip.ai/security\n  status: 200\n  keywords: [iso 42001, iso 27001, soc 2 type ii, gdpr, \"\\xA7203 stgb\", hipaa, nist\n      800-53, zero data retention]\n  quote: >-\n    \"We also adhere to strict industry standards, including certifications like\n    ISO 27001, SOC 2 Type II, and HIPAA.\"\nnotes: >-\n  Superset of an automated probe pass that had reduced this file to four\n  certifications sourced only from the marketing security page. HIPAA is a real\n  published claim (verified in prose on /security); ISO 42001 and §203 StGB are\n  named in the certification band on the same page; the trust center itself is a\n  Vanta-hosted single-page app at trust.deepip.ai, which serves an HTML shell for\n  every path including /.well-known/security.txt.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepip/refs/heads/main/security/deepip-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, ISO 42001, HIPAA, GDPR
tags:
- Company
- Intellectual Property
- Patents
- Legal Tech
- Artificial Intelligence
- Patent Drafting
- IP Management
- Document Automation
- Security
- MCP
- Agents
- Prior Art Search
trust_url: https://trust.deepip.ai/
---
