---
certifications:
- ISO/IEC 27001 (ISMS)
- PrivacyMark (JIS Q 15001)
- PCI DSS
- SOC 1 Type 1
- SOC 2 Type 1
description: ''
kind: trust-center
layout: security
name: Super Studio Trust Center
name_suffix: Trust Center
overview: SUPER STUDIO maintains a public trust center documenting ISO/IEC 27001 (ISMS), PrivacyMark (JIS Q 15001), PCI DSS, SOC 1 Type 1, and SOC 2 Type 1 compliance.
provider_name: SUPER STUDIO
provider_slug: super-studio
slug: super-studio-trust-center
source_filename: super-studio-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://ec-force.com/security\nnote: >-\n  probe-security-programs.py returned vdp=none trust=none — it found no security.txt, no bug-bounty\n  listing and no recognised trust-center platform. That is correct: SUPER STUDIO runs no automated\n  trust portal. What it does publish is a first-party security page naming real certifications, so\n  this artifact is written by hand from that page and marked searched rather than probed.\ntrust_center:\n  platform: none (first-party page)\n  url: https://ec-force.com/security\n  machine_readable: false\n  document_downloads: false\n  note: >-\n    No Vanta/Drata/SafeBase-style portal, no downloadable SOC report request flow, and no\n    certificate registration numbers are published. Certifications are stated as prose claims.\ncertifications:\n- name: ISO/IEC 27001 (ISMS)\n  status: certified (claimed)\n  registration_number: not published\n- name: PrivacyMark (JIS Q 15001)\n  status:\
  \ certified (claimed)\n  registration_number: not published\n- name: PCI DSS\n  status: compliant (claimed)\n  scope: credit card processing\n  level: not published\n- name: SOC 1 Type 1\n  status: report obtained (claimed)\n  report_access: not published\n- name: SOC 2 Type 1\n  status: report obtained (claimed)\n  report_access: not published\n  note: >-\n    Type 1, not Type 2 — a point-in-time design opinion rather than an operating-effectiveness\n    opinion over a period. Recorded exactly as stated.\ncontrols_published:\n- encryption at rest at the database level\n- TLS in transit\n- periodic third-party vulnerability assessment\n- two-factor authentication for admin accounts\n- IP address restriction for admin access\n- all customer data stored within Japan\n- supplier security review process\n- annual information-security training, new hires within 5 days\n- background/reference checks at hire\n- confidentiality agreements with employees and suppliers\ndata_residency:\n  region:\
  \ Japan\n  claim: All customer data is managed exclusively within Japan.\nvulnerability_disclosure:\n  program: none found\n  security_txt: absent\n  probed:\n  - url: https://ec-force.com/.well-known/security.txt\n    status: 404\n  - url: https://www.super-studio.jp/.well-known/security.txt\n    status: 404\n  - url: https://agent.ec-force.com/.well-known/security.txt\n    status: 404\n  bug_bounty: none found on HackerOne, Bugcrowd or Intigriti\n  note: >-\n    No VulnerabilityDisclosure artifact is written and no `Security` pointer is claimed, because\n    there is no published intake path for a security report. SUPER STUDIO states it commissions\n    third-party vulnerability assessments; it publishes no way for an outside researcher to report\n    one.\n  remediation: >-\n    Serve /.well-known/security.txt (RFC 9116) on ec-force.com and super-studio.jp naming a Contact\n    and a Policy URL. It is the cheapest single item on this page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-studio/refs/heads/main/security/super-studio-trust-center.yml
summary_line: ISO/IEC 27001 (ISMS), PrivacyMark (JIS Q 15001), PCI DSS, SOC 1 Type 1, SOC 2 Type 1
tags:
- Company
- E-Commerce
- Commerce
- Subscription Commerce
- Order Management
- Marketing Automation
- Business Intelligence
- Software-as-a-Service
- Artificial Intelligence
- Agents
- MCP
- Japan
trust_url: ''
---
