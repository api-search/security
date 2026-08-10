---
certifications:
- ISO/IEC 27001:2022
- O-TTPS (ISO/IEC 20243:2023)
- SOC 1 Type II
- SOC 2 Type II
- TISAX AL3
- EU-US Data Privacy Framework
- Veracode Verified
description: Onapsis publishes its certification and attestation posture on a public "Compliance Resources" page rather than a trust.<domain> subdomain, which is why the automated trust-center probe recorded nothing (trust.onapsis.com has no DNS record). The page names each certification, its scope, and how the underlying report is obtained. Audit reports themselves are customer-gated and released on request.
kind: trust-center
layout: security
name: Onapsis Trust Center
name_suffix: Trust Center
overview: Onapsis maintains a public trust center documenting ISO/IEC 27001:2022, O-TTPS (ISO/IEC 20243:2023), SOC 1 Type II, SOC 2 Type II, TISAX AL3, EU-US Data Privacy Framework, and Veracode Verified compliance.
provider_name: Onapsis
provider_slug: onapsis
slug: onapsis-trust-center
source_filename: onapsis-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nprobe: true\nsource: https://onapsis.com/compliance-resources/\nurl: https://onapsis.com/compliance-resources/\ndescription: >-\n  Onapsis publishes its certification and attestation posture on a public\n  \"Compliance Resources\" page rather than a trust.<domain> subdomain, which is\n  why the automated trust-center probe recorded nothing (trust.onapsis.com has\n  no DNS record). The page names each certification, its scope, and how the\n  underlying report is obtained. Audit reports themselves are customer-gated\n  and released on request.\ncertifications:\n- name: ISO/IEC 27001:2022\n  since: 2019\n  scope: The Onapsis Platform and Onapsis Cloud Platform — software development, client implementation, customer experience\n  availability: reports available to Onapsis customers on request\n  verification: https://www.certipedia.com/quality_marks/9108653165?locale=en\n- name: O-TTPS (ISO/IEC 20243:2023)\n  body: The Open Group\n  scope:\
  \ The Onapsis Platform product lifecycle — design, sourcing, build, fulfillment, distribution, sustainment, disposal\n  note: Supply-chain integrity standard for commercial ICT products\n- name: SOC 1 Type II\n  body: AICPA\n  availability: reports available to Onapsis customers on request\n- name: SOC 2 Type II\n  body: AICPA\n  availability: reports available to Onapsis customers on request\n- name: TISAX AL3\n  scope: Germany region assessment (automotive industry)\n  enx_portal_id: S3T76N\n  assessment_id: ATZW9P-3\n  availability: available to Onapsis customers on request\n- name: EU-US Data Privacy Framework\n  kind: self-assessment certification\n- name: Veracode Verified\n  since: 2020\n  kind: application security program verification\nrecognitions:\n- name: SAP Endorsed App\n  note: The Onapsis Platform is listed as an SAP Endorsed App and available in the SAP Store.\nreport_access:\n  audit_reports: ISO 27001, SOC 1/SOC 2 Type II and TISAX results are released to Onapsis customers\
  \ on request.\n  public_pages:\n  - https://onapsis.com/compliance-resources/\n  - https://onapsis.com/quality-policy/\nevidence:\n- source: https://onapsis.com/compliance-resources/\n  kind: compliance/certifications page\n  http_status: 200\n  keywords: [iso 27001, soc 1 type ii, soc 2 type ii, tisax, o-ttps, eu-us data privacy framework, veracode verified]\n- source: https://trust.onapsis.com/\n  kind: trust subdomain probe\n  http_status: null\n  note: no DNS record\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onapsis/refs/heads/main/security/onapsis-trust-center.yml
summary_line: ISO/IEC 27001:2022, O-TTPS (ISO/IEC 20243:2023), SOC 1 Type II, SOC 2 Type II, TISAX AL3, EU-US Data Privacy Framework, Veracode Verified
tags:
- Company
- Cybersecurity
- Application Security
- Vulnerability Management
- Compliance
- SAP
- ERP
- Threat Detection
- GraphQL
- Enterprise Software
trust_url: https://onapsis.com/compliance-resources/
---
