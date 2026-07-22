---
certifications:
- SOC 2 Type II
- GDPR
- CCPA
description: Klarity operates a Vanta-hosted Trust Center at trust.klarity.ai where customers and prospects request the SOC 2 Type II report and supporting security documentation. The public-facing summary of that posture lives on the Trust & Safety page at klarity.ai/legal/trust-and-safety, which is the source for the certifications and controls captured here.
kind: trust-center
layout: security
name: Klarity Trust Center
name_suffix: Trust Center
overview: Klarity maintains a public trust center documenting SOC 2 Type II, GDPR, and CCPA compliance.
provider_name: Klarity
provider_slug: klarity
slug: klarity-trust-center
source_filename: klarity-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: false\nsource: https://www.klarity.ai/legal/trust-and-safety\nurl: https://trust.klarity.ai/\ndescription: >-\n  Klarity operates a Vanta-hosted Trust Center at trust.klarity.ai where\n  customers and prospects request the SOC 2 Type II report and supporting\n  security documentation. The public-facing summary of that posture lives on the\n  Trust & Safety page at klarity.ai/legal/trust-and-safety, which is the source\n  for the certifications and controls captured here.\nplatform: Vanta\ncertifications:\n  - {name: SOC 2 Type II, availability: on request via trust center, note: Verified through independent audit with continuous monitoring.}\n  - {name: GDPR, kind: regulatory compliance}\n  - {name: CCPA, kind: regulatory compliance, docs: https://www.klarity.ai/legal/ccpa}\ncontrols:\n  encryption_in_transit: HTTPS/TLS\n  encryption_at_rest: AES-256\n  access_control: Least-privilege, role-restricted production access protected\
  \ by MFA.\n  penetration_testing: Recurring third-party penetration testing.\n  ai_subprocessors: Zero-data-retention agreements with AI subprocessors.\n  data_deletion: On-demand deletion, propagated permanently to backups.\nreport_access:\n  soc_reports: Requested through the Vanta-hosted trust center at https://trust.klarity.ai/.\nsecurity_contact:\n  email: security@klarity.ai\n  source: DNS CAA iodef record for klarity.ai (see security/klarity-domain-security.yml)\n  note: >-\n    Published as the CAA incident-reporting address. Klarity does not publish a\n    /.well-known/security.txt, a responsible-disclosure policy, or a bug-bounty\n    program, so no VulnerabilityDisclosure artifact was written.\ndocs:\n  - https://www.klarity.ai/legal/trust-and-safety\n  - https://www.klarity.ai/legal/subprocessors\n  - https://www.klarity.ai/legal/genai-usage-policy\n  - https://www.klarity.ai/legal/privacy-policy\nevidence:\n  - source: https://www.klarity.ai/legal/trust-and-safety\n    keywords:\
  \ [soc 2 type ii, gdpr, ccpa, aes-256, penetration testing, trust center]\n  - source: https://trust.klarity.ai/\n    status: 200\n    keywords: [vanta, klarity trust center]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klarity/refs/heads/main/security/klarity-trust-center.yml
summary_line: SOC 2 Type II, GDPR, CCPA
tags:
- Company
- Artificial Intelligence
- Business Process Management
- Process Intelligence
- Enterprise Software
- Document Automation
- Finance
- Governance Risk and Compliance
- Agents
trust_url: https://trust.klarity.ai/
---
