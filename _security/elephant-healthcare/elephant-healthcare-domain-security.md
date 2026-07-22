---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: elephant.healthcare
  spf: true
hosts:
- cert_expires: Sep  9 14:04:00 2026 GMT
  host: elephant.healthcare
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elephant Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elephant Healthcare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Elephant Healthcare
provider_slug: elephant-healthcare
slug: elephant-healthcare-domain-security
source_filename: elephant-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elephant.healthcare\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 14:04:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: elephant.healthcare\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elephant-healthcare/refs/heads/main/security/elephant-healthcare-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Health Tech
- Electronic Health Records
- EHR
- Digital Health
- Public Health
- Africa
- Interoperability
- Primary Care
---
