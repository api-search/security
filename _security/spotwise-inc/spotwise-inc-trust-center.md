---
certifications: []
description: ''
kind: trust-center
layout: security
name: Spotwise Inc Trust Center
name_suffix: Trust Center
overview: Spotwise, Inc. maintains a public trust center covering its security and compliance posture.
provider_name: Spotwise, Inc.
provider_slug: spotwise-inc
slug: spotwise-inc-trust-center
source_filename: spotwise-inc-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nprobe: true\nsource: https://spotwise.ai/security\nurl: https://spotwise.ai/security\n# CAUTION FOR FUTURE RUNS: probe-security-programs.py keyword-matches \"SOC 2\" and\n# \"ISO 27001\" out of Spotwise's NEGATION of them and writes certifications:\n# [SOC 2, ISO 27001, GDPR]. That is wrong and has been reverted twice (2026-07-21,\n# 2026-08-12). Spotwise holds NO completed certification. If the automated probe\n# clobbers this file again, restore this version.\ncertifications: []\nposture:\n  formal_certifications: none\n  in_progress:\n  - name: SOC 2 Type II\n    status: in-progress\n    certified: false\n  - name: ISO/IEC 27001\n    status: in-progress\n    certified: false\n  disclaimed:\n  - SOC 2\n  - ISO 27001\n  frameworks:\n  - GDPR (self-attested alignment; EU-based company)\n  - EU AI Act (stated alignment ahead of full application on 2026-08-02)\n  practices:\n  - sensible security practices\n  - access controls\n  - customer\
  \ knowledge scoped to the customer workspace; not used to train shared\n    models and not shared with other broadcasters\n  security_contact: security@spotwise.ai\n  enterprise_review: handled by direct correspondence rather than a published trust\n    portal\nquotes:\n- source: https://spotwise.ai/security\n  text: >-\n    You will not find SOC 2 or ISO certification logos on this page. We have not\n    completed those certifications.\n- source: https://spotwise.ai/faq\n  text: >-\n    Not yet - SOC 2 Type II and ISO 27001 are both in progress, and we are aligning\n    with the EU AI Act ahead of its full application on 2 August 2026. Until an auditor\n    signs each one off we say so plainly, and we will not show you a badge we have not\n    earned.\nrating_pointer_note: >-\n  No `type: Compliance` pointer is emitted. `compliance_published` credits a published\n  compliance programme with named certifications; Spotwise explicitly states it holds\n  none. The `TrustCenter` pointer stands\
  \ on its own — the page is real and unusually\n  candid, but candour about absent certifications is not a certification.\nevidence:\n- source: https://spotwise.ai/security\n  keywords:\n  - data & privacy\n  - gdpr\n  - access controls\n  note: SOC 2 / ISO explicitly stated as NOT completed\n- source: https://spotwise.ai/faq\n  status: 200\n  note: FAQ upgrades the posture from \"not completed\" to \"in progress\" for both SOC 2\n    Type II and ISO 27001, and adds EU AI Act alignment\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotwise-inc/refs/heads/main/security/spotwise-inc-trust-center.yml
summary_line: trust center published
tags:
- Company
- Broadcast Media
- Advertising
- Media Monitoring
- Sales Intelligence
- Lead Generation
- Artificial Intelligence
- Radio
- Model Context Protocol
- Agents
- Attribution
trust_url: https://spotwise.ai/security
---
