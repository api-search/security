---
certifications:
- SOC 2 Type II
- CSA STAR Level 1
description: ''
kind: trust-center
layout: security
name: Retail Zipline Trust Center
name_suffix: Trust Center
overview: Retail Zipline maintains a public trust center documenting SOC 2 Type II and CSA STAR Level 1 compliance.
provider_name: Retail Zipline
provider_slug: retail-zipline
slug: retail-zipline-trust-center
source_filename: retail-zipline-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://trust.getzipline.com/\nsummary: >-\n  Zipline runs a public trust center at trust.getzipline.com, hosted on Vanta.\n  The page is a client-rendered single-page application, so its certification\n  list is not readable without executing JavaScript — every path under the host\n  returns the same 5,436-byte HTML shell. The certifications below are therefore\n  taken from Zipline's own published pages and announcements rather than scraped\n  from the trust center.\ntrust_center:\n  url: https://trust.getzipline.com/\n  resources_url: https://trust.getzipline.com/resources\n  vendor: Vanta\n  http_status: 200\n  machine_readable: false\n  note: >-\n    SPA catch-all — /.well-known/agent-card.json, /llms.txt, /api/trust-center\n    and an arbitrary nonexistent path all return the identical 200 HTML shell.\n    None of those are documents and none were credited.\ncertifications:\n- name: SOC 2 Type II\n  status: certified\n\
  \  source: https://getzipline.com/blog/retail-zipline-receives-soc-2-type-ii-certification/\n- name: CSA STAR Level 1\n  status: self-assessment completed\n  source: https://getzipline.com/security/\nprivacy_programs:\n- GDPR\n- CCPA\ndocuments:\n- name: Data Processing Addendum\n  url: https://getzipline.com/data-processing-addendum/\n- name: Security Addendum\n  url: https://getzipline.com/security-addendum/\n- name: Data Subject Access Form\n  url: https://getzipline.com/data-subject-access-form/\n- name: Privacy Policy\n  url: https://getzipline.com/privacy-policy/\nx-evidence:\n- url: https://trust.getzipline.com/\n  http_status: 200\n  fetched: '2026-08-26'\n- url: https://trust.getzipline.com/resources\n  http_status: 200\n  fetched: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retail-zipline/refs/heads/main/security/retail-zipline-trust-center.yml
summary_line: SOC 2 Type II, CSA STAR Level 1
tags:
- Retail
- Retail Operations
- Task Management
- Employee Communications
- Store Operations
- Workforce
- Knowledge Base
- Software-as-a-Service
- MCP
- Company
trust_url: ''
---
