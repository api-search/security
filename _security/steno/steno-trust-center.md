---
certifications:
- SOC 2 Type II
- HIPAA
description: ''
kind: trust-center
layout: security
name: Steno Trust Center
name_suffix: Trust Center
overview: Steno maintains a public trust center documenting SOC 2 Type II and HIPAA compliance.
provider_name: Steno
provider_slug: steno
slug: steno-trust-center
source_filename: steno-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nprobe: true\nurl: https://trust.steno.com/\nplatform: Vanta Trust Center\nplatform_evidence: served HTML carries assets.vanta.com stylesheets and data-signature-manifest-url\n  on https://assets.vanta.com/static/signature-manifest.*.json\nscope: Steno Connect, Firm Dashboard, and Ops\ncertifications:\n- name: SOC 2 Type II\n  trust_service_criteria:\n  - Security\n  - Availability\n  - Confidentiality\n  auditor: Linford & Company LLP\n  source: https://brief.steno.com/soc2-hipaa-compliance\n- name: HIPAA\n  note: audited for compliance with the Health Insurance Portability and Accountability\n    Act of 1996 as a business associate handling protected health information in transcripts\n    and proceedings\n  auditor: Linford & Company LLP\n  source: https://brief.steno.com/soc2-hipaa-compliance\ncontinuous_monitoring:\n  vendor: Vanta\n  note: continuous control monitoring with real-time alerting and automated evidence\n    collection,\
  \ per Steno's published compliance post\nrelated_pages:\n- url: https://trust.steno.com/resources\n  status: 200\n  note: trust center resource list (Vanta-hosted, client-side rendered)\n- url: https://help.steno.com/safety-and-security\n  status: 200\n  note: '\"Is Steno Connect Safe And Secure?\" knowledge-base article'\n- url: https://steno.com/dpa\n  status: 200\n  note: Data Processing Addendum\nvulnerability_disclosure: null\nvulnerability_disclosure_note: 'no vulnerability disclosure program found: /.well-known/security.txt\n  returns 404 on steno.com and 403 on api.steno.com, and steno.com/security returns\n  404. The Vanta trust center is client-side rendered so any report-a-vulnerability\n  link it carries was not readable anonymously.'\nx-evidence:\n- url: https://trust.steno.com/\n  http_status: 200\n  content_type: text/html\n  observed: '<title>Steno Trust Center</title> + <link rel=\"canonical\" href=\"https://trust.steno.com\">'\n- url: https://brief.steno.com/soc2-hipaa-compliance\n\
  \  http_status: 200\n  observed: names SOC 2 Type II (Security, Availability, Confidentiality), HIPAA, auditor\n    Linford & Company LLP, and Vanta continuous monitoring\n- url: https://steno.com/.well-known/security.txt\n  http_status: 404\n- url: https://steno.com/security\n  http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steno/refs/heads/main/security/steno-trust-center.yml
summary_line: SOC 2 Type II, HIPAA
tags:
- Company
- Legal
- Legal Technology
- Court Reporting
- Depositions
- Litigation Support
- Transcription
- Video
- Artificial Intelligence
- Salesforce
trust_url: https://trust.steno.com/
---
