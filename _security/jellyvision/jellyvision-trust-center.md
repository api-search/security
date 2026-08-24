---
certifications:
- SOC 2
- HIPAA
description: ''
kind: trust-center
layout: security
name: Jellyvision Trust Center
name_suffix: Trust Center
overview: Jellyvision maintains a public trust center documenting SOC 2 and HIPAA compliance.
provider_name: Jellyvision
provider_slug: jellyvision
slug: jellyvision-trust-center
source_filename: jellyvision-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://trust.jellyvision.com/\nurl: https://trust.jellyvision.com/\nstatus: 200\nsecondary_source: https://www.jellyvision.com/security/\ncertifications:\n- name: SOC 2\n  source: https://www.jellyvision.com/security/\n- name: HIPAA\n  source: https://www.jellyvision.com/security/\nreadable: false\nreadability_note: >-\n  A real, provider-operated trust center is served at https://trust.jellyvision.com/ (HTTP 200,\n  ~92KB). It is an Angular single-page application — the served HTML loads\n  apps/trustcenter/main.086bf7365dda6143.js plus polyfills and a stylesheet, and its entire static\n  body text is the two words \"Trust Center\". No certification name, framework, subprocessor list,\n  document index, contact address or vendor marker (SafeBase / Vanta / Drata / Conveyor / Whistic /\n  Secureframe) survives without JavaScript execution, and the JS bundle exposes no readable API base\n  to fetch the underlying data from.\
  \ The certifications recorded above are therefore read from the\n  statically rendered Data Security & Privacy Commitment page, not from the trust center itself.\n  For a machine reader, this trust center is effectively empty.\naudits:\n  internal_security_audits: true\n  source: https://www.jellyvision.com/security/\n  note: >-\n    The security page cites internal security audits and over a decade of healthcare technology\n    experience. No third-party penetration test report, audit letter or bridge letter is published\n    at a public URL.\nevidence:\n- url: https://trust.jellyvision.com/\n  status: 200\n  note: Angular SPA shell; body text is \"Trust Center\" only\n- url: https://trust.jellyvision.com/apps/trustcenter/main.086bf7365dda6143.js\n  status: 200\n  note: 141664 bytes; no https API base and no trust-platform vendor string found\n- url: https://www.jellyvision.com/security/\n  status: 200\n  note: Data Security & Privacy Commitment; names SOC2 and HIPAA\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jellyvision/refs/heads/main/security/jellyvision-trust-center.yml
summary_line: SOC 2, HIPAA
tags:
- Company
- Employee Benefits
- Human Resources
- Benefits Administration
- Benefits Enrollment
- Health Insurance
- Decision Support
- HR Technology
- Insurance
- Employee Engagement
trust_url: https://trust.jellyvision.com/
---
