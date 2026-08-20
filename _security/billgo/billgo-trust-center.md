---
certifications:
- SOC 2 Type II
- SOC 1 Type I
- PCI DSS Level 1 (via service providers)
description: ''
kind: trust-center
layout: security
name: Billgo Trust Center
name_suffix: Trust Center
overview: BillGO maintains a public trust center documenting SOC 2 Type II, SOC 1 Type I, and PCI DSS Level 1 (via service providers) compliance.
provider_name: BillGO
provider_slug: billgo
slug: billgo-trust-center
source_filename: billgo-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: searched\nprobe: true\nsource: https://billgo.com/security\nurl: https://billgo.com/security\ntrust_center_hosted: false\ntrust_center_note: >-\n  BillGO has no dedicated trust centre — trust.billgo.com and security.billgo.com do not\n  resolve. The compliance posture is prose on a marketing page at billgo.com/security;\n  no attestation report, SOC package request flow, or third-party verification portal\n  is offered.\ncertifications:\n- SOC 2 Type II\n- SOC 1 Type I\n- PCI DSS Level 1 (via service providers)\nclaims:\n- name: SOC 2 Type II\n  statement: BillGO undergoes annual SOC 1 Type I and SOC 2 Type II audits to ensure its\n    security controls meet industry standards.\n- name: SOC 1 Type I\n  statement: BillGO undergoes annual SOC 1 Type I and SOC 2 Type II audits to ensure its\n    security controls meet industry standards.\n- name: PCI DSS Level 1\n  statement: BillGO Exchange partners with PCI-compliant Level 1 Service providers\
  \ — the\n    highest standard.\n  scope_note: The stated Level 1 compliance belongs to BillGO's service providers; the page\n    does not claim a BillGO Level 1 attestation.\n- name: TLS 1.2+\n  statement: Transport Layer Security (TLS 1.2+) to protect data in transit.\nsecurity_program:\n  mfa: Multi-factor authentication enabled for all accounts.\n  ddos: Advanced anti-bot services protect our servers.\n  monitoring: Round-the-clock monitoring for suspicious activity.\n  sdlc: Development team adheres to a rigorous SDLC process.\nvulnerability_disclosure:\n  public_program: false\n  bug_bounty: private\n  statement: '...supported by a private bug bounty program.'\n  policy_url: null\n  security_contact: null\n  security_txt: false\n  note: >-\n    A private bug bounty is stated but there is no public disclosure policy, no\n    security@ contact, and no /.well-known/security.txt on any BillGO host, so an\n    outside researcher has no published route to report a finding. Recorded here\
  \ rather\n    than as a VulnerabilityDisclosure artifact, because there is no reachable channel to\n    record.\nevidence:\n- source: https://billgo.com/security\n  status: 200\n  keywords:\n  - soc 2 type ii\n  - soc 1 type i\n  - pci\n  - bug bounty\n  - tls 1.2\n- source: https://trust.billgo.com/\n  status: 0\n  note: DNS does not resolve\n- source: https://billgo.com/.well-known/security.txt\n  status: 404\nx-evidence:\n  fetched: '2026-08-07'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billgo/refs/heads/main/security/billgo-trust-center.yml
summary_line: SOC 2 Type II, SOC 1 Type I, PCI DSS Level 1 (via service providers)
tags:
- Payments
- Bill Pay
- Financial-Services
- Banking
- ACH
- Virtual Cards
- Fintech
- GraphQL
trust_url: https://billgo.com/security
---
