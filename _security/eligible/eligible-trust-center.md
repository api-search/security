---
certifications:
- HITRUST r2
- HITRUST CSF
- NIST Cybersecurity Framework v1.1
- SOC 2
- CAQH CORE Phase I
- CAQH CORE Phase II
- CAQH CORE Phase III
- CAQH CORE Phase IV
- EHNAC HNAP
- EHNAC CEAP
- HIPAA
description: ''
kind: trust-center
layout: security
name: Eligible Trust Center
name_suffix: Trust Center
overview: Eligible maintains a public trust center documenting HITRUST r2, HITRUST CSF, NIST Cybersecurity Framework v1.1, SOC 2, CAQH CORE Phase I, CAQH CORE Phase II, CAQH CORE Phase III, CAQH CORE Phase IV, EHNAC HNAP, EHNAC CEAP, and HIPAA compliance.
provider_name: Eligible
provider_slug: eligible
slug: eligible-trust-center
source_filename: eligible-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: false\nsource: https://eligible.com/compliance\nurl: https://eligible.com/compliance\nnote: >-\n  The mechanical probe (0-working/probe-security-programs.py) recorded no trust\n  center, and it was right to: https://eligible.com/compliance is a client-rendered\n  single-page app whose served HTML contains no body text for a keyword match to find.\n  The page IS real, and the served <head> carries the claim verbatim in its meta\n  description — \"Industry proven, we are certified by: SOC2, HiTrust, CAQH, NIST.\" —\n  which is what this artifact is written from, together with Eligible's own dated\n  certification announcements captured in blogs/. Recorded as searched rather than\n  probed for that reason.\ncertifications:\n  - HITRUST r2\n  - HITRUST CSF\n  - NIST Cybersecurity Framework v1.1\n  - SOC 2\n  - CAQH CORE Phase I\n  - CAQH CORE Phase II\n  - CAQH CORE Phase III\n  - CAQH CORE Phase IV\n  - EHNAC HNAP\n  - EHNAC CEAP\n\
  \  - HIPAA\nevidence:\n  - source: https://eligible.com/compliance\n    status: 200\n    kind: meta-description\n    keywords: [soc2, hitrust, caqh, nist]\n    note: >-\n      Page title \"Compliance\". Body content is JavaScript-rendered; only the head is\n      readable without executing scripts.\n  - source: https://eligible.com/security\n    status: 200\n    kind: alias\n    note: /security serves the same Compliance page.\n  - source: https://eligible.com/blog/eligible-achieves-hitrust-r2-certification/\n    kind: announcement\n    date: '2026-06-23'\n    note: HITRUST r2 + NIST CSF v1.1 for the Platform Services System.\n  - source: https://eligible.com/blog/eligible-achieves-phase-i-ii-iii-and-iv-caqh-core-certification/\n    kind: announcement\n    date: '2024-09-17'\n  - source: https://eligible.com/blog/eligible-attains-hitrust-csf-certification/\n    kind: announcement\n    date: '2022-02-16'\n  - source: https://eligible.com/blog/eligible-achieves-ehnac-cloud-enabled-accreditation/\n\
  \    kind: announcement\n    date: '2018-01-18'\n  - source: https://eligible.com/blog/soc2-certification-exceptional-year-without-exceptions/\n    kind: announcement\n    date: '2017-11-09'\ngaps:\n  - No dedicated trust portal (trust.eligible.com does not resolve).\n  - No downloadable or gated report request flow found on the public surface.\n  - No subprocessor list, no data-residency statement, no penetration-test summary.\n  - >-\n    The compliance claims are only machine-readable as a meta description; the page a\n    security reviewer would actually read requires a browser.\ndetail: see conformance/eligible-conformance.yml for the dated, per-certification record\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eligible/refs/heads/main/security/eligible-trust-center.yml
summary_line: HITRUST r2, HITRUST CSF, NIST Cybersecurity Framework v1.1, SOC 2, CAQH CORE Phase I, CAQH CORE Phase II, CAQH CORE Phase III, CAQH CORE Phase IV, EHNAC HNAP, EHNAC CEAP, HIPAA
tags:
- Billing
- Eligibility
- Healthcare
- Insurance
- Claims
trust_url: https://eligible.com/compliance
---
