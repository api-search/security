---
certifications: []
description: ''
kind: trust-center
layout: security
name: Theorg Trust Center
name_suffix: Trust Center
overview: The Org maintains a public trust center covering its security and compliance posture.
provider_name: The Org
provider_slug: theorg
slug: theorg-trust-center
source_filename: theorg-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://theorg.com/trust\nurl: https://theorg.com/trust\ncertifications: []\ncertifications_in_progress:\n- name: ISO 27001/2\n  status: in-progress\n  claim: 'We are enhancing our security controls to be aligned with ISO 27001/2'\n- name: SOC 2\n  status: in-progress\n  claim: 'Independent third-party audits to achieve SOC 2 certification.'\ncertification_note: >-\n  CORRECTION APPLIED. The mechanical probe extracted \"SOC 2\" and \"ISO 27001\" as held\n  certifications from keyword matching. Reading the page shows both are ASPIRATIONAL: the\n  copy is \"We are enhancing our security controls to be aligned with ISO 27001/2, and\n  SOC-2 certification\" and \"Independent third-party audits to achieve SOC 2 certification\".\n  No attestation, report, certificate, audit date or auditor is published, and there is no\n  gated trust portal to request one from. Recording these as achieved would credit The Org\n  with\
  \ a compliance posture it has not claimed, so certifications[] is empty and NO\n  `Compliance` pointer is emitted in apis.yml.\nscope_of_program:\n  controls: Security, Availability, Confidentiality\n  claim: 'Robust controls to uphold Security, Availability, and Confidentiality.'\n  reviews: 'Ongoing reviews to ensure compliance with data privacy laws and regulations.'\nprivacy_posture:\n  data_sourcing:\n  - Monitoring of team pages on company websites for leadership changes\n  - News aggregation — press releases and announcements about new hires and promotions\n  - Tracking of updates and changes to public LinkedIn profiles\n  - User generated content from professionals maintaining their own public org chart\n  claim: >-\n    'We only process public professional data, regardless of where an individual is based,\n    across all of our solutions.'\n  subject_controls:\n  - Join your company and edit contact/position pages\n  - Report wrong information via the report function\n  - Opt\
  \ out of appearing on The Org\n  opt_out_url: https://theorg.com/do-not-sell\n  opt_out_label: Do not sell or share my information\n  note: >-\n    Relevant to this provider specifically: the product is a people-data platform built\n    substantially from third-party public data, so the trust page functions as a data-subject\n    rights surface as much as a security one. No GDPR, CCPA or HIPAA program is named,\n    and no subprocessor list is published.\nlegal_entity: Orgio, Inc.\ncertifications_source: https://theorg.com/trust\nevidence:\n- source: https://theorg.com/trust\n  http_status: 200\n  keywords: [iso 27001, soc 2, trust center, privacy, security controls]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theorg/refs/heads/main/security/theorg-trust-center.yml
summary_line: trust center published
tags:
- Company
- Organizational Charts
- People Data
- Sales Intelligence
- Prospecting
- Org Chart
- B2B Data
- MCP
- Contact Data
- Lead Generation
- Job
- Agents
trust_url: https://theorg.com/trust
---
