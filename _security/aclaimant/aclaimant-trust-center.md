---
api_specs:
- filename: aclaimant-platform-api-openapi.json
  format: json
  label: Aclaimant Platform API
  slug: aclaimant-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aclaimant/refs/heads/main/openapi/aclaimant-platform-api-openapi.json
certification_count: 3
certifications:
- SOC 2
- GDPR
- Penetration test report
description: ''
kind: trust-center
layout: security
name: Aclaimant Trust Center
name_suffix: Trust Center
overview: Aclaimant maintains a public trust center documenting SOC 2, GDPR, and Penetration test report compliance.
provider_name: Aclaimant
provider_slug: aclaimant
slug: aclaimant-trust-center
source_filename: aclaimant-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://trust.aclaimant.com/\nurl: https://trust.aclaimant.com/\nname: Aclaimant Trust Center\nhost: trust.aclaimant.com\nplatform: Vanta\nplatform_evidence: >-\n  trust.aclaimant.com is a CNAME to 5c4f6013f5ea8a08d7799d36.cname.vantatrust.com; the page loads the Vanta\n  trust-report bundle from assets.vanta.com and carries the document link https://app.vanta.com/doc?s=0peek5mgfa7elxxs7ragx4\nmachine_readable: false\nmachine_readable_note: >-\n  The trust center renders client-side. Anonymous GET of https://trust.aclaimant.com/ returns a 6.5KB HTML\n  shell whose only readable text is the title \"Aclaimant Trust Center\"; no certification list, control list or\n  subprocessor list is present in the served markup, and the Vanta trust-report API returns 401 to anonymous\n  callers. The certifications below are therefore taken from Aclaimant's own published support article, not\n  from this page.\ncertifications:\n- name: SOC\
  \ 2\n  status: held-per-provider-statement\n  published: false\n  access: request\n  evidence: https://support.aclaimant.com/hc/en-us/articles/13754454190363-SOC-2-and-IT-Compliance-Information-Request\n  note: >-\n    Aclaimant's support article \"SOC 2 and IT Compliance Information Request\" states that SOC 2 compliance\n    information and a SOC 2 bridge letter are available to customers on request via a linked form. The report\n    itself is not published; no attestation document or period is publicly readable.\n- name: GDPR\n  status: statement-available-on-request\n  published: false\n  access: request\n  evidence: https://support.aclaimant.com/hc/en-us/articles/13754454190363-SOC-2-and-IT-Compliance-Information-Request\n  note: The same article lists a \"GDPR Compliance Statement\" among the documents released on request.\n- name: Penetration test report\n  status: available-on-request\n  published: false\n  access: request\n  evidence: https://support.aclaimant.com/hc/en-us/articles/13754454190363-SOC-2-and-IT-Compliance-Information-Request\n\
  misattribution_guard: >-\n  https://www.aclaimant.com/security lists \"ISO 27001, SSAE16 SOC-1 Type II/ISAE 3402, SOC 2 - Security, SOC 3,\n  PCI Level 1 and FISMA moderate\" but attributes them explicitly to Aclaimant's INFRASTRUCTURE PARTNERS\n  (\"Our infrastructure partners hold one or more of the following accreditations\"), not to Aclaimant. Those\n  accreditations are deliberately NOT recorded as Aclaimant certifications here.\nevidence:\n- url: https://trust.aclaimant.com/\n  status: 200\n  note: Vanta-hosted trust center, title \"Aclaimant Trust Center\", JS-rendered\n- url: https://support.aclaimant.com/hc/en-us/articles/13754454190363-SOC-2-and-IT-Compliance-Information-Request\n  status: 200\n  note: fetched through the Zendesk Help Center API (support.aclaimant.com/api/v2/help_center)\n- url: https://www.aclaimant.com/security\n  status: 200\n  note: security protocols FAQ; accreditations listed there belong to infrastructure partners\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aclaimant/refs/heads/main/security/aclaimant-trust-center.yml
summary_line: SOC 2, GDPR, Penetration test report
tags:
- Risk Management
- Insurance
- Claims Management
- Incident Management
- Safety
- RMIS
- Workers Compensation
- OSHA
- Enterprise Risk Management
- Insurtech
trust_url: https://trust.aclaimant.com/
---
