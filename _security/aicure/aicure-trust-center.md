---
certification_count: 2
certifications:
- ISO/IEC 27001
- SOC 2
description: ''
kind: trust-center
layout: security
name: Aicure Trust Center
name_suffix: Trust Center
overview: AiCure maintains a public trust center documenting ISO/IEC 27001 and SOC 2 compliance.
provider_name: AiCure
provider_slug: aicure
slug: aicure-trust-center
source_filename: aicure-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://aicure.com/company/data-privacy-security\nname: AiCure trust and compliance page\ntrust_center:\n  exists: true\n  form: marketing-page\n  url: https://aicure.com/company/data-privacy-security\n  status: 200\n  portal: false\n  portal_note: >-\n    This is a page on the corporate site, not a trust portal. There is no Vanta/Drata/SafeBase\n    instance, no document request flow and no subprocessor list; trust.aicure.com does not resolve\n    (NXDOMAIN).\ncertifications:\n- name: ISO/IEC 27001\n  claimed: true\n  certificate_published: false\n  auditor_published: false\n  validity_published: false\n- name: SOC 2\n  claimed: true\n  report_published: false\n  report_availability: >-\n    AiCure states SOC 2 reports \"are restricted to specified parties with sufficient knowledge and\n    understanding of the service organization's system\" - available on request, not published.\n  trust_service_criteria_named:\n  - security\n\
  \  - availability\n  - processing integrity\n  - confidentiality\n  - privacy\nregulatory_compliance:\n- HIPAA\n- GDPR\n- 21 CFR Part 11\ndata_practices_published:\n- claim: All data is encrypted when collected and maintained encrypted at all times, in motion and\n    at rest.\n- claim: >-\n    AiCure analyses each country of deployment and either makes the required filings or assists the\n    CRO/sponsor in making them.\n- claim: >-\n    Full facial images are retained only on AiCure's secure servers, encrypted at all times, with\n    access limited to a small group of trained and certified video reviewers.\nprivacy_policy: https://aicure.com/privacy-policy\nterms_of_service: https://aicure.com/terms-of-use\ngaps:\n- No security.txt on any host (see well-known/aicure-well-known.yml).\n- No vulnerability disclosure policy, bug bounty or security contact page was found.\n- No DNSSEC and no CAA records on aicure.com (see security/aicure-domain-security.yml).\n- 'DMARC is published but the\
  \ policy is p=none, so nothing is quarantined or rejected.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aicure/refs/heads/main/security/aicure-trust-center.yml
summary_line: ISO/IEC 27001, SOC 2
tags:
- Company
- Healthcare
- Clinical Trials
- Medication Adherence
- Digital Biomarkers
- Digital Health
- Artificial Intelligence
- Computer-Vision
- Patient Engagement
- Life Sciences
- Open-Source
trust_url: ''
---
