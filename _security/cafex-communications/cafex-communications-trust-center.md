---
certifications:
- ISO 27001
- SOC 2
- ISO 42001
description: ''
kind: trust-center
layout: security
name: Cafex Communications Trust Center
name_suffix: Trust Center
overview: CafeX Communications maintains a public trust center documenting ISO 27001, SOC 2, and ISO 42001 compliance.
provider_name: CafeX Communications
provider_slug: cafex-communications
slug: cafex-communications-trust-center
source_filename: cafex-communications-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nprobe: true\nurl: https://trust.cafex.ai/\naliases:\n- https://trust.cafex.com/\nplatform: Vanta Trust Center\nplatform_note: >-\n  The trust center is a Vanta-hosted, client-rendered single-page app (assets.vanta.com,\n  data-slugid mksnhe97jw17qxrzg8553). Its certification list is not present in the served HTML, so\n  the certifications below are taken from CafeX's own published security datasheet and the\n  compliance badges rendered on cafex.ai — not inferred from the trust center shell.\ncertifications:\n- name: ISO 27001\n  source: https://cafex.ai/asset/svg/iso-27001.svg\n  also: https://support.cafex.com/support/solutions/articles/73000179994-cafex-security-datasheet\n- name: SOC 2\n  source: https://cafex.ai/asset/svg/soc-2.svg\n- name: ISO 42001\n  source: https://cafex.ai/asset/svg/iso-42001.svg\n  note: AI management system standard\nregulatory_posture:\n- name: HIPAA\n  statement: Executes Business Associate Agreements\
  \ (BAA) with covered entities.\n- name: GDPR / UK data protection\n  statement: Registered with the UK Information Commissioner's Office (ICO).\n- name: EU-U.S. Data Privacy Framework\n  statement: Complies with the EU-U.S. DPF, the UK Extension, and the Swiss-U.S. DPF.\nsecurity_practices:\n  hosting: Amazon Web Services (AWS)\n  encryption_in_transit: Industry best-practice protocols between users and CafeX servers.\n  encryption_at_rest: >-\n    Encrypted at rest on AWS, with runtime field-level encryption, dual key management and\n    tenant-specific keys.\n  penetration_testing: Third-party penetration testing experts engaged.\n  vulnerability_scanning: Regular dynamic vulnerability scanning plus static code analysis of source repositories.\n  identity: SSO and MFA supported; tenants can enforce their own MFA policies.\ncontacts:\n  compliance: compliance@cafex.com\ndocuments:\n- name: CafeX Security Datasheet\n  url: https://support.cafex.com/support/solutions/articles/73000179994-cafex-security-datasheet\n\
  \  access: public\nevidence:\n- source: https://trust.cafex.ai/\n  http_status: 200\n  keywords:\n  - trust center\n  - security\n  - privacy\n  - compliance\n- source: https://support.cafex.com/support/solutions/articles/73000179994-cafex-security-datasheet\n  http_status: 200\n  keywords:\n  - iso 27001\n  - hipaa\n  - gdpr\n  - data privacy framework\n- source: https://cafex.ai/\n  http_status: 200\n  keywords:\n  - iso-27001\n  - soc-2\n  - iso-42001\nx-evidence:\n  fetched: '2026-08-08'\n  control_probe:\n    url: https://bogus-control-xyz.cafex.ai/\n    result: NXDOMAIN\n    note: no wildcard DNS, so trust.cafex.ai resolving is a real host and not a catch-all\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cafex-communications/refs/heads/main/security/cafex-communications-trust-center.yml
summary_line: ISO 27001, SOC 2, ISO 42001
tags:
- Company
- Low-Code
- Workflow Automation
- Agentic AI
- Audit and Compliance
- Collaboration
- Enterprise Software
- Regulated Industries
- Process Automation
trust_url: https://trust.cafex.ai/
---
