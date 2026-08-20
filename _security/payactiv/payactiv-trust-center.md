---
certifications:
- SOC 2
- ISO 27001
- PCI DSS
- CCPA
- Visa Service Provider
- Certified B Corporation
description: ''
kind: trust-center
layout: security
name: Payactiv Trust Center
name_suffix: Trust Center
overview: PayActiv maintains a public trust center documenting SOC 2, ISO 27001, PCI DSS, CCPA, Visa Service Provider, and Certified B Corporation compliance.
provider_name: PayActiv
provider_slug: payactiv
slug: payactiv-trust-center
source_filename: payactiv-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nprobe: true\nsource: https://payactiv.com/trust-center/\nurl: https://payactiv.com/trust-center/\ncertifications:\n- SOC 2\n- ISO 27001\n- PCI DSS\n- CCPA\n- Visa Service Provider\n- Certified B Corporation\nprograms:\n- name: Information Security Program\n  url: https://payactiv.com/information-security-program/\n  summary: >-\n    Policies, procedures and standards maintained in accordance with PCI/SOC/ISO controls. Publishes\n    encryption at rest and in transit, mandatory multi-factor authentication, annual security training,\n    employee background checks, an incident response plan with a reporting mechanism for suspected\n    vulnerabilities, and log retention of 180 days minimum (one year for confidential data).\n- name: Data Processing Agreement\n  url: https://payactiv.com/data-processing-agreement/\n  summary: California Consumer Privacy Act compliant data processing terms.\n- name: Privacy Policy\n  url: https://payactiv.com/privacy-policy/\n\
  - name: Compliance Handbook\n  url: https://www.payactiv.com/trust-center/compliance-handbook\n  summary: EWA program compliance with state and federal wage-and-labor and consumer-protection law.\ntesting:\n  external_penetration_test: at least annually\n  internal_penetration_test: twice yearly by an independent third party\n  internal_vulnerability_scans: monthly minimum\n  external_vulnerability_scans: quarterly minimum, via a PCI Approved Scanning Vendor\n  remediation_sla: critical and high severity remediated within 30 days\nlicensing:\n  nmls_id: '2591928'\n  ewa_licenses:\n  - 'Wisconsin Department of Financial Institutions — EWA license 2591928EWA'\n  - 'Connecticut Department of Banking — small loan license SLC-2591928'\n  - 'Nevada Financial Institution Division — EWA license EWA00009'\nevidence:\n- source: https://payactiv.com/trust-center/\n  http_status: 200\n  keywords: [soc 2, iso 27001, pci dss, ccpa, visa service provider, trust center, b corporation]\n- source: https://payactiv.com/information-security-program/\n\
  \  http_status: 200\n  keywords: [pci, soc, iso, encryption, incident response, penetration test]\nnotes: >-\n  No public vulnerability disclosure policy, bug bounty program, or security@ contact was found.\n  /.well-known/security.txt returns 404 on payactiv.com; the only published contact is the general\n  support address, so no VulnerabilityDisclosure artifact or Security pointer was emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payactiv/refs/heads/main/security/payactiv-trust-center.yml
summary_line: SOC 2, ISO 27001, PCI DSS, CCPA, Visa Service Provider, Certified B Corporation
tags:
- Company
- Financial-Services
- Earned Wage Access
- Payments
- Payroll
- Human Resources
- Cards
- Financial Wellness
- Fintech
trust_url: https://payactiv.com/trust-center/
---
