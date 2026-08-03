---
api_specs:
- filename: threatlocker-portal-openapi-original.json
  format: json
  label: ThreatLocker PortalAPI
  slug: threatlocker-portalapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-portal-openapi-original.json
certifications:
- SOC 2 Type II
- ISO 27001
- FedRAMP
description: ''
kind: trust-center
layout: security
name: Threatlocker Trust Center
name_suffix: Trust Center
overview: ThreatLocker maintains a public trust center documenting SOC 2 Type II, ISO 27001, and FedRAMP compliance.
provider_name: ThreatLocker
provider_slug: threatlocker
slug: threatlocker-trust-center
source_filename: threatlocker-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nprobe: true\nsource: >-\n  https://threatlocker.kb.help/threatlocker-security-and-privacy/, https://threatlocker.kb.help/compliance/,\n  https://www.threatlocker.com/software-security-audit\nurl: https://threatlocker.kb.help/threatlocker-security-and-privacy/\ndedicated_trust_center: false\nnote: >-\n  ThreatLocker publishes no trust.threatlocker.com or /trust page — trust.threatlocker.com does not\n  resolve and www.threatlocker.com/security and /compliance both 404. Its security and compliance\n  posture is published inside the Help Center instead. The automated probe\n  (0-working/probe-security-programs.py) therefore returned trust=none; this file records the posture\n  found by manual search of the pages ThreatLocker actually publishes.\ncertifications:\n- {name: SOC 2 Type II, status: certified, detail: 'Security controls audited at least annually by an independent AICPA-certified auditor; the SOC 2 Type II report is available\
  \ to customers on request under NDA'}\n- {name: ISO 27001, status: in-progress, detail: 'Stated in progress as of March 2026; ThreatLocker states ISO 27001/2 compliance in its security documentation'}\n- {name: FedRAMP, status: instance-published, detail: 'A dedicated \"Portal [Instance FedRAMP]\" component is published on the public status page'}\npractices:\n  encryption: All confidential information, including data transmitted to and from the ThreatLocker agent, is encrypted in transit and at rest using industry-standard encryption protocols.\n  penetration_testing: ThreatLocker undergoes regular internal and external penetration tests.\n  data_residency: Regionally isolated instances (AE1, AU1, CA1, EU1, SA1 and lettered US/global instances) with per-instance portal and API hosts.\nvulnerability_disclosure:\n  found: false\n  policy: null\n  contact: null\n  bug_bounty: null\n  note: >-\n    NO vulnerability disclosure program, responsible-disclosure policy, published security contact,\
  \ or\n    bug bounty was found — notable for a security vendor. /.well-known/security.txt returns 404 on\n    every ThreatLocker host, and /security, /responsible-disclosure and /vulnerability-disclosure all\n    404 on www.threatlocker.com. No HackerOne, Bugcrowd or Intigriti program was found. No `Security`\n    or `VulnerabilityDisclosure` pointer is wired in apis.yml because nothing is published; this is a\n    verified absence, not an untested one.\n  probes:\n  - {url: 'https://www.threatlocker.com/.well-known/security.txt', http_status: 404}\n  - {url: 'https://www.threatlocker.com/security.txt', http_status: 404}\n  - {url: 'https://portalapi.threatlocker.com/.well-known/security.txt', http_status: 404}\n  - {url: 'https://threatlocker.kb.help/.well-known/security.txt', http_status: 404}\n  - {url: 'https://www.threatlocker.com/responsible-disclosure', http_status: 404}\n  - {url: 'https://www.threatlocker.com/vulnerability-disclosure', http_status: 404}\nframeworks_page: https://threatlocker.kb.help/compliance/\n\
  audit_report_page: https://www.threatlocker.com/software-security-audit\nevidence:\n- {source: 'https://threatlocker.kb.help/threatlocker-security-and-privacy/', http_status: 200, keywords: [soc 2 type ii, iso 27001, encryption, penetration test, cmmc level 2, hipaa]}\n- {source: 'https://threatlocker.kb.help/compliance/', http_status: 200, keywords: [nist, cmmc, pci-dss, iso 27001 annex a, hipaa security rule, cis controls]}\n- {source: 'https://www.threatlocker.com/software-security-audit', http_status: 200}\n- {source: 'https://trust.threatlocker.com/', http_status: 0, result: does-not-resolve}\n- {source: 'https://www.threatlocker.com/security', http_status: 404}\n- {source: 'https://www.threatlocker.com/compliance', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/security/threatlocker-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, FedRAMP
tags:
- cybersecurity
- zero-trust
- endpoint-security
- application-control
- allowlisting
- ransomware-prevention
- privileged-access-management
- network-access-control
- managed-detection-and-response
- device-management
- msp
- compliance
trust_url: https://threatlocker.kb.help/threatlocker-security-and-privacy/
---
