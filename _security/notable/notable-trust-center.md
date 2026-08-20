---
certifications:
- SOC 2 Type 2
- ISO/IEC 27001:2022
- PCI DSS
- HITRUST
description: ''
kind: trust-center
layout: security
name: Notable Trust Center
name_suffix: Trust Center
overview: Notable maintains a public trust center documenting SOC 2 Type 2, ISO/IEC 27001:2022, PCI DSS, and HITRUST compliance.
provider_name: Notable
provider_slug: notable
slug: notable-trust-center
source_filename: notable-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nprobe: true\nsource: https://trust.notablehealth.com/\nurl: https://trust.notablehealth.com/\nplatform: SafeBase (notablehealth.portals.safebase.io)\ncertifications:\n- SOC 2 Type 2\n- ISO/IEC 27001:2022\n- PCI DSS\n- HITRUST\ncontrols:\n- name: Penetration Testing\n  detail: Penetration tests are conducted on an annual basis.\n  maturity: full\nsecurity_mailbox: security@notablehealth.com\nevidence:\n- source: https://trust.notablehealth.com/\n  status: 200\n  keywords:\n  - soc 2 type 2\n  - iso/iec 27001:2022\n  - pci dss\n  - hitrust\n  - penetration testing\n  - trust center\n- source: https://www.notablehealth.com/security\n  status: 200\n  note: redirects to https://trust.notablehealth.com/\nnote: >-\n  Certification strings are recorded verbatim as the Trust Center renders them.\n  The 2026-08-15 run of probe-security-programs.py generalized these to \"SOC 2\" /\n  \"ISO 27001\" and dropped HITRUST; the fuller verbatim list\
  \ was restored per the\n  never-downgrade rule. HIPAA compliance is claimed by Notable on its own site and\n  in its llms.txt but is not a certification badge on the Trust Center, so it is\n  carried in conformance/notable-conformance.yml rather than here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notable/refs/heads/main/security/notable-trust-center.yml
summary_line: SOC 2 Type 2, ISO/IEC 27001:2022, PCI DSS, HITRUST
tags:
- Company
- Application
- Healthcare
- Artificial Intelligence
- Automation
- Revenue Cycle
- Patient Access
- Agents
- Prior Authorization
- EHR Integration
- FHIR
- Contact Center
- Care Operations
trust_url: https://trust.notablehealth.com/
---
