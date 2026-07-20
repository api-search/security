---
api_specs:
- filename: leaseaccelerator-api-openapi.yml
  format: yaml
  label: LeaseAccelerator API
  slug: leaseaccelerator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseaccelerator/refs/heads/main/openapi/leaseaccelerator-api-openapi.yml
certifications:
- SOC 2 Type 2
- SOC 1 Type 2
- ISO 27001
- ISO 9001
description: insightsoftware operates a Conveyor-hosted trust center covering its full product portfolio, including LeaseAccelerator. Certifications below are the programs insightsoftware itself declares on the trust center (the `certifications` list in the trust center's own payload), corroborated by the public insightsoftware.com/trust/ summary page. LeaseAccelerator-specific audit reports and bridge letters are published in the trust center data room; access is gated behind an NDA/request flow.
kind: trust-center
layout: security
name: Leaseaccelerator Trust Center
name_suffix: Trust Center
overview: LeaseAccelerator maintains a public trust center documenting SOC 2 Type 2, SOC 1 Type 2, ISO 27001, and ISO 9001 compliance.
provider_name: LeaseAccelerator
provider_slug: leaseaccelerator
slug: leaseaccelerator-trust-center
source_filename: leaseaccelerator-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://trust.insightsoftware.com/, https://insightsoftware.com/trust/\nurl: https://trust.insightsoftware.com/\ndescription: >-\n  insightsoftware operates a Conveyor-hosted trust center covering its full product portfolio, including\n  LeaseAccelerator. Certifications below are the programs insightsoftware itself declares on the trust\n  center (the `certifications` list in the trust center's own payload), corroborated by the public\n  insightsoftware.com/trust/ summary page. LeaseAccelerator-specific audit reports and bridge letters are\n  published in the trust center data room; access is gated behind an NDA/request flow.\nscope: >-\n  Company-wide (insightsoftware), with per-product audit reports. LeaseAccelerator has its own SOC 1 Type 2\n  and SOC 2 Type 2 reports rather than being covered only by a corporate report.\nvendor: Conveyor\ncertifications:\n- name: SOC 2 Type 2\n  scope: product\n  note: >-\n\
  \    Annual SOC 2 Type 2 audits evaluating design and operating effectiveness of internal controls, based on\n    AICPA Trust Services Principles and Criteria for Security, Availability, and Confidentiality.\n- name: SOC 1 Type 2\n  scope: product\n- name: ISO 27001\n  scope: company\n  note: Information security management system (ISMS) certification.\n- name: ISO 9001\n  scope: company\n  note: Quality management system; a 2025 re-certification document is published (ISO 9001:2015).\nregulatory:\n- GDPR\n- CCPA\nleaseaccelerator_documents:\n  note: >-\n    Document titles observed in the trust center data room listing that name LeaseAccelerator or its Lease\n    Accounting Manager (LAM) product. Documents themselves require a request; only their existence and\n    titles are public.\n  documents:\n  - LeaseAccelerator Lease Accounting Manager - SOC 2 Type 2 - Audit Report 2026\n  - LeaseAccelerator LAM - SOC 1 Type 2 - Audit Report 2026\n  - LeaseAccelerator - SOC 2 Type 2 Audit Report\
  \ April 2025\n  - LeaseAccelerator - SOC 1 Type 2 Audit Report April 2025\n  - LeaseAccelerator SOC 1 Type 2 Audit Report Sep 2025\n  - LeaseAccelerator - Agreed Upon Procedures - Report 2025\n  - 2025 Lease Accounting Manager Customer Facing (penetration test report)\n  bridge_letters: >-\n    Monthly SOC 1 Type 2 and SOC 2 Type 2 bridge letters are published continuously; the most recent\n    observed are dated July 2026.\nroadmap:\n  note: Published on the trust center as planned compliance work.\n  items:\n  - ISO 27001 - 2026 certificate\n  - JustPerform - Account Reconciliation - SOC 1 Type 2\nsecurity_program:\n  source: https://insightsoftware.com/trust/\n  approach: defense in depth\n  practices:\n  - Encryption — TLS in transit, AES-256 at rest.\n  - Vulnerability management with scheduled scans and dark web monitoring.\n  - Secure software development lifecycle with static code analysis and independent third-party penetration testing.\n  - Documented incident response plan covering\
  \ reporting, roles and responsibilities, prioritization, escalation, and remediation.\n  - Employee security awareness training and phishing simulations.\n  - Automated encrypted backups with disaster recovery plans.\n  - >-\n    Security remediations from penetration testing and automated vulnerability scanning are shipped in\n    platform releases (see the 26.2.1 release notes).\n  breach_notification: >-\n    Upon becoming aware of a Security Incident, insightsoftware will notify the customer without undue\n    delay and will provide information relating to the incident as it becomes known or is reasonably\n    requested.\nevidence:\n- source: https://trust.insightsoftware.com/\n  finding: >-\n    Trust center payload declares certifications iso-9001, iso-27001, soc1-type-2, soc2-type-2, ccpa, gdpr;\n    data room lists LeaseAccelerator-specific SOC 1/SOC 2 Type 2 audit reports and monthly bridge letters.\n- source: https://insightsoftware.com/trust/\n  finding: >-\n    Public trust\
  \ summary names ISO 27001, SSAE-18 SOC 2 Type 2, GDPR, and CCPA, and describes the security\n    program above.\nnotes:\n- >-\n  ISO 27017, ISO 27018, FedRAMP, PCI DSS, HIPAA, TISAX, and CSA STAR strings appear in the trust center\n  page source but belong to the Conveyor platform's generic certification label vocabulary, not to\n  insightsoftware's declared certification set. They are deliberately excluded here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaseaccelerator/refs/heads/main/security/leaseaccelerator-trust-center.yml
summary_line: SOC 2 Type 2, SOC 1 Type 2, ISO 27001, ISO 9001
tags:
- Company
- Lease Accounting
- Lease Administration
- Financial Reporting
- Enterprise Software
- Accounting
- Real Estate
- Asset Management
- ERP Integration
- Compliance
trust_url: https://trust.insightsoftware.com/
---
