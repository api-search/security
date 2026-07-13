---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uottawa.ca
  spf: true
hosts:
- cert_expires: Aug 11 17:30:56 2026 GMT
  host: www.uottawa.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  7 23:59:59 2026 GMT
  host: ruor.uottawa.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Ottawa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Ottawa, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Ottawa
provider_slug: university-of-ottawa
slug: university-of-ottawa-domain-security
source_filename: university-of-ottawa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uottawa.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 17:30:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ruor.uottawa.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uottawa.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-ottawa/refs/heads/main/security/university-of-ottawa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Canada
- Bilingual
- Library
- Institutional Repository
- DSpace
- OAI-PMH
- Open Access
---
