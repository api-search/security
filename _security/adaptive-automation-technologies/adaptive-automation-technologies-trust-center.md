---
certification_count: 1
certifications:
- SOC 2 Type II
description: Adaptive publishes its own security posture as a narrative page at https://adaptive.live/security rather than as a hosted trust portal. A host at trust.adaptive.live resolves but answers HTTP 403 behind a Cloudflare bot challenge to every client tried, so its contents could not be read and nothing is asserted about it.
kind: trust-center
layout: security
name: Adaptive Automation Technologies Trust Center
name_suffix: Trust Center
overview: Adaptive Automation Technologies maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Adaptive Automation Technologies
provider_slug: adaptive-automation-technologies
slug: adaptive-automation-technologies-trust-center
source_filename: adaptive-automation-technologies-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://adaptive.live/security\ndescription: >-\n  Adaptive publishes its own security posture as a narrative page at\n  https://adaptive.live/security rather than as a hosted trust portal. A host at\n  trust.adaptive.live resolves but answers HTTP 403 behind a Cloudflare bot challenge to\n  every client tried, so its contents could not be read and nothing is asserted about it.\nurl: https://adaptive.live/security\nprogram_sections:\n- Secure Personnel — background checks, NDAs, security training\n- Secure Development — secure SDLC, design review, OWASP Top 10, annual secure-coding training\n- Secure Testing — third-party penetration testing and vulnerability scanning of all\n  production and internet-facing systems, plus SAST and DAST including open-source libraries\n- Cloud Security — per-customer trust-zone isolation, unique encryption keys, encryption at\n  rest and in transit, role-based and least-privilege access\n- Compliance\
  \ — external certification\ncertifications:\n- name: SOC 2 Type II\n  body: AICPA\n  auditor: Prescient Assurance\n  status: completed\n  evidence: >-\n    \"Adaptive Automation Technologies successfully completed the AICPA Service Organization\n    Control (SOC) 2 Type II audit.\" — https://adaptive.live/security\n  report_access: On request; the page directs report requests to debarshi@adaptive.live.\nmisattribution_note: >-\n  The words HIPAA, GDPR and CSA STAR also appear on this page, but ONLY inside the\n  description of the auditor (Prescient Assurance) and its other service lines — they are\n  NOT claimed as Adaptive's own certifications. They are deliberately excluded from\n  certifications[] above. Adaptive's product separately helps CUSTOMERS track SOC 2, ISO\n  27001, HIPAA, PCI-DSS and GDPR control posture (see the Compliance module in\n  https://documentation.adaptive.live/platform/compliance); those are product features, not\n  Adaptive's own attestations, and are recorded\
  \ in conformance/ as such.\nx-evidence:\n- url: https://adaptive.live/security\n  http_status: 200\n  fetched: '2026-09-07'\n- url: https://trust.adaptive.live/\n  http_status: 403\n  fetched: '2026-09-07'\n  note: Cloudflare bot challenge; contents unreadable, nothing asserted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-automation-technologies/refs/heads/main/security/adaptive-automation-technologies-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Company
- Security
- Privileged Access Management
- Identity and Access Management
- Data Security
- Agents
- Model Context Protocol
- Infrastructure
- Databases
- Kubernetes
- Compliance
- Audit
trust_url: https://adaptive.live/security
---
