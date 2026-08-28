---
certifications:
- ISO/IEC 27001:2022
- SOC 2 Type II
- HIPAA
description: ''
kind: trust-center
layout: security
name: Navina Trust Center
name_suffix: Trust Center
overview: Navina maintains a public trust center documenting ISO/IEC 27001:2022, SOC 2 Type II, and HIPAA compliance.
provider_name: Navina
provider_slug: navina
slug: navina-trust-center
source_filename: navina-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://trust.navina.ai/\nnote: >-\n  Navina operates a public trust center. It is an Angular single-page app served\n  by Anecdotes, so the certification list is rendered client-side and is not\n  present in the served HTML — the certifications recorded here therefore come\n  from Navina's own dated announcement pages rather than from scraping the trust\n  center body. The automated probe (probe-security-programs.py) reported\n  trust=none for exactly this reason: it keyword-matches the response body and\n  the body is an empty app shell. This file corrects that miss by hand, with\n  evidence.\n\ntrust_center:\n  present: true\n  url: https://trust.navina.ai/\n  http_status: 200\n  platform: Anecdotes\n  platform_evidence: 'og:title meta tag reads \"Trust Center | Powered by Anecdotes\"'\n  rendering: >-\n    Client-side Angular. HTML shell is 92,685 bytes and contains no certification\n    names; the app bundle at /apps/trustcenter/main.*.js\
  \ exposes no anonymous\n    data endpoint that could be read without executing the app.\n\ncertifications:\n- name: ISO/IEC 27001:2022\n  status: certified\n  detail: Fourth consecutive year of certification, under the 2022 revision.\n  source: https://www.navina.ai/news/navina-achieves-iso-27001-certification-again\n  published: '2024-04-11'\n- name: SOC 2 Type II\n  status: audited\n  detail: >-\n    Security, availability and confidentiality criteria; \"no deviation on all\n    controls\". Auditor described only as a Big Four firm.\n  source: https://www.navina.ai/news/successful-soc-2-type-ii-hipaa-audit\n  published: '2024-03-14'\n- name: HIPAA\n  status: audited\n  detail: HIPAA audit completed alongside the SOC 2 Type II engagement.\n  source: https://www.navina.ai/news/successful-soc-2-type-ii-hipaa-audit\n  published: '2024-03-14'\n\ndocument_access:\n  self_serve: unknown\n  note: >-\n    Whether audit reports are downloadable, NDA-gated, or request-only could not\n    be determined\
  \ without executing the client-side app. Not asserted either way.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navina/refs/heads/main/security/navina-trust-center.yml
summary_line: ISO/IEC 27001:2022, SOC 2 Type II, HIPAA
tags:
- Company
- Healthcare
- Artificial Intelligence
- Clinical Decision Support
- Value-Based Care
- Risk Adjustment
- Electronic Health Records
- FHIR
- Interoperability
- Medical Coding
trust_url: ''
---
