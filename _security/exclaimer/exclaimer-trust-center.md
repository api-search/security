---
api_specs:
- filename: exclaimer-subscriptions-openapi.yml
  format: yaml
  label: Exclaimer Cloud API
  slug: exclaimer-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exclaimer/refs/heads/main/openapi/exclaimer-subscriptions-openapi.yml
certifications:
- SOC 2 Type II
- ISO/IEC 27001
- ISO/IEC 27018
- PCI DSS
- CSA (Cloud Security Alliance)
- Cyber Essentials
- HIPAA
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Exclaimer Trust Center
name_suffix: Trust Center
overview: Exclaimer maintains a public trust center documenting SOC 2 Type II, ISO/IEC 27001, ISO/IEC 27018, PCI DSS, CSA (Cloud Security Alliance), Cyber Essentials, HIPAA, GDPR, and CCPA compliance.
provider_name: Exclaimer
provider_slug: exclaimer
slug: exclaimer-trust-center
source_filename: exclaimer-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://exclaimer.com/product/security/\nurl: https://trust.exclaimer.com/\ncompliance_page: https://exclaimer.com/product/security/\ntrust_center_platform: Conveyor\ntrust_center_note: >-\n  trust.exclaimer.com returns HTTP 200 but is a client-side rendered Conveyor\n  trust-portal shell; no certification text is present in the served HTML. The\n  certification list below is therefore taken from Exclaimer's own security page\n  at https://exclaimer.com/product/security/, which states each claim in prose.\ncertifications:\n- name: SOC 2 Type II\n  claim: certified\n  detail: SOC 2 Type II certified by the AICPA for security, availability, and confidentiality.\n- name: ISO/IEC 27001\n  claim: certified\n  detail: Certified ISMS covering management of sensitive data.\n- name: ISO/IEC 27018\n  claim: certified\n  detail: Certified for protection of personally identifiable information (PII) in the cloud.\n- name: PCI\
  \ DSS\n  claim: self-certified\n  detail: >-\n    Self-certified against PCI DSS via an annually reviewed self-assessment\n    questionnaire; card payments are handled by a PCI DSS-certified third-party\n    provider so cardholder data is not processed by Exclaimer directly.\n- name: CSA (Cloud Security Alliance)\n  claim: certified\n  detail: Certified by the Cloud Security Alliance following an independent assessment of cloud service security controls.\n- name: Cyber Essentials\n  claim: certified\n  detail: Certified under the UK government-backed Cyber Essentials scheme managed by the NCSC.\n- name: HIPAA\n  claim: compliant\n  detail: States HIPAA compliance for handling protected health information (PHI).\n- name: GDPR\n  claim: compliant\n  detail: States full compliance with the EU General Data Protection Regulation.\n- name: CCPA\n  claim: compliant\n  detail: States adherence to the California Consumer Privacy Act of 2018 and other U.S. privacy laws.\nnot_claimed:\n- name: FedRAMP\n\
  \  note: >-\n    An automated keyword probe of trust.exclaimer.com matched \"FedRAMP\" inside the\n    Conveyor platform's own boilerplate/JS payload, not in any Exclaimer claim.\n    Exclaimer's security page does not mention FedRAMP. Recorded here so a later\n    re-run does not re-introduce it as a certification.\nevidence:\n- source: https://exclaimer.com/product/security/\n  http_status: 200\n  kind: provider security/compliance page (server-rendered prose)\n  keywords:\n  - soc 2 type ii\n  - iso/iec 27001 & 27018\n  - pci dss\n  - csa\n  - cyber essentials\n  - hipaa\n  - gdpr\n  - ccpa\n- source: https://trust.exclaimer.com/\n  http_status: 200\n  kind: trust center portal (Conveyor; JS-rendered, no certification text in HTML)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exclaimer/refs/heads/main/security/exclaimer-trust-center.yml
summary_line: SOC 2 Type II, ISO/IEC 27001, ISO/IEC 27018, PCI DSS, CSA (Cloud Security Alliance), Cyber Essentials, HIPAA, GDPR, CCPA
tags:
- Company
- Email
- Email Signatures
- Email Signature Management
- Microsoft-365
- Google Workspace
- Marketing
- Productivity
- Software-as-a-Service
- Security
trust_url: https://trust.exclaimer.com/
---
