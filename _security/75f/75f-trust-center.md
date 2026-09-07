---
certification_count: 2
certifications:
- SOC 2
- VAPT
description: ''
kind: trust-center
layout: security
name: 75F Trust Center
name_suffix: Trust Center
overview: 75F maintains a public trust center documenting SOC 2 and VAPT compliance.
provider_name: 75F
provider_slug: 75f
slug: 75f-trust-center
source_filename: 75f-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nprobe: true\nprobe_result: >-\n  0-working/probe-security-programs.py returned trust=none because it checks trust.<domain>,\n  security.<domain> and <domain>/trust|/security|/compliance, and 75F's page is at /software/security/.\n  https://www.75f.io/security 301-redirects there and was fetched and read by hand (HTTP 200), which is\n  why this file is method: searched rather than probed.\nurl: https://www.75f.io/software/security/\ncertifications:\n- name: SOC 2\n  claim: >-\n    \"75F is proud to join the list of leading organizations that have achieved SOC 2 compliance.\" The\n    page describes SOC 2 as the AICPA guidelines covering security, availability, processing integrity,\n    confidentiality and privacy.\n  report_available: false\n  auditor_named: false\n- name: VAPT\n  claim: >-\n    75F states it is \"VAPT Certified\" — vulnerability assessment and penetration testing, described as a\n    rigorous process probing the system's\
  \ security measures and resilience against breaches.\n  report_available: false\n  auditor_named: false\nframeworks:\n- name: O.R.A.N.G.E. Security Framework\n  claim: >-\n    75F's own named set of protocols for securing building control systems, data, applications and\n    networks.\nevidence:\n- source: https://www.75f.io/software/security/\n  http_status: 200\n  keywords: [soc 2, vapt, penetration]\ngaps:\n  no_trust_portal: true\n  no_subprocessor_list: true\n  no_public_audit_report: true\n  note: >-\n    There is no trust.75f.io or security.75f.io host (both fail to resolve), no downloadable attestation,\n    no named auditor and no subprocessor list. The claims are marketing-page assertions; a buyer's\n    security team would have to request the SOC 2 report through sales.\nvulnerability_disclosure:\n  found: false\n  probed:\n  - {url: 'https://www.75f.io/.well-known/security.txt', status: 404}\n  - {url: 'https://75f.io/.well-known/security.txt', status: 301}\n  - {url: 'https://api.75f.io/.well-known/security.txt',\
  \ status: 404}\n  - {url: 'https://www.75f.io/responsible-disclosure', status: 404}\n  - {url: 'https://www.75f.io/security/responsible-disclosure', status: 404}\n  - {url: 'https://www.75f.io/vulnerability-disclosure', status: 404}\n  - {url: 'https://hackerone.com/75f', status: 404}\n  - {url: 'https://bugcrowd.com/75f', status: 404}\n  note: >-\n    No security.txt, no responsible-disclosure page, no bug bounty program and no published security\n    contact address. No security/75f-vulnerability-disclosure.yml is written and no `Security` pointer is\n    emitted in apis.yml, because there is nothing to point at. For a vendor whose API physically actuates\n    HVAC equipment in occupied commercial buildings, this is the single most consequential gap in the\n    profile — a researcher who finds a flaw has no published route to report it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/75f/refs/heads/main/security/75f-trust-center.yml
summary_line: SOC 2, VAPT
tags:
- Company
- Building Automation
- Smart Buildings
- HVAC
- Internet of Things
- Energy Management
- Project Haystack
- Facilities Management
- Sensors
- Building Management System
trust_url: https://www.75f.io/software/security/
---
