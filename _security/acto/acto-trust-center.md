---
certification_count: 4
certifications:
- SOC 2 Type 2
- ISO/IEC 27001
- GDPR
- FDA 21 CFR Part 11
description: ''
kind: trust-center
layout: security
name: Acto Trust Center
name_suffix: Trust Center
overview: ACTO maintains a public trust center documenting SOC 2 Type 2, ISO/IEC 27001, GDPR, and FDA 21 CFR Part 11 compliance.
provider_name: ACTO
provider_slug: acto
slug: acto-trust-center
source_filename: acto-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nprobe: true\nsource: https://trust.acto.com/\nurl: https://trust.acto.com/\nplatform: SafeBase\nplatform_evidence: >-\n  trust.acto.com is a CNAME to acto.portals.safebase.io — a first-party subdomain ACTO\n  controls, delegated to the SafeBase trust-center product.\ncertifications:\n- SOC 2 Type 2\n- ISO/IEC 27001\n- GDPR\n- FDA 21 CFR Part 11\nevidence:\n- source: https://trust.acto.com/\n  status: 200\n  keywords:\n  - soc 2 type 2\n  - iso/iec 27001\n  - gdpr\n  - 21 cfr part 11\n  - trust center\n  note: >-\n    Certification list read from the rendered trust-center page. The host is behind a\n    Cloudflare bot challenge and answers 403 to a plain command-line fetch, so the page was\n    read with a browser-class client; it is live, not dead.\n- source: https://acto.com/platform/\n  status: 200\n  note: >-\n    Corroborates the 21 CFR Part 11 claim independently — \"validated closed and open\n    systems, secure user authentication,\
  \ time-stamped audit trails, change control\n    processes\".\nreadability: rendered-read\nvulnerability_disclosure:\n  found: false\n  partial: true\n  note: >-\n    The trust center carries an \"App Security\" section listing a \"Responsible Disclosure\"\n    document, but the document itself sits inside the SafeBase portal behind a document\n    access request and could not be read anonymously, so no policy URL and no security\n    contact can be recorded. The automated probe (0-working/probe-security-programs.py)\n    correctly declined to write a vulnerability-disclosure artifact on this evidence.\n  probed:\n  - url: https://acto.com/.well-known/security.txt\n    status: 404\n  - url: https://acto.com/security\n    status: 404\n  - url: https://acto.com/responsible-disclosure\n    status: 404\n  - url: https://acto.com/vulnerability-disclosure\n    status: 404\n  - url: https://app.acto.com/.well-known/security.txt\n    status: 404\n  pointer_policy: >-\n    NO Security and NO VulnerabilityDisclosure\
  \ pointer is emitted. There is no publicly\n    readable disclosure policy or security contact to point at, and pointing at the trust\n    center root for a document we could not open would be a claim we cannot back.\npointer_policy: >-\n  A TrustCenter pointer is emitted against security/acto-trust-center.yml, and a Compliance\n  pointer against https://trust.acto.com/ — ACTO names four current, verifiable frameworks\n  there, which is exactly what compliance_published reads.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acto/refs/heads/main/security/acto-trust-center.yml
summary_line: SOC 2 Type 2, ISO/IEC 27001, GDPR, FDA 21 CFR Part 11
tags:
- Life Sciences
- Pharmaceutical
- Sales Enablement
- Learning Management
- Field Force Effectiveness
- Medical Affairs
- Commercial Excellence
- Training and Certification
- Omnichannel Engagement
- Artificial Intelligence
- Medical Devices
- Biotechnology
- Content Management
- Healthcare
trust_url: https://trust.acto.com/
---
